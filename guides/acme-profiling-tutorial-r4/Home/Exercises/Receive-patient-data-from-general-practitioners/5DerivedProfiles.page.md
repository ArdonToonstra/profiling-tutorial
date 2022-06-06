---
topic: Derivedprofiles
---
# Step 5: Derived profiles ⛓️

<ul class="roundbox">
<p>Hospital X operates in the United States of America. Their API must be compatible with the US-Core profiles. On top of the US-Core profile for Immunization, it has additional requirements. </p>
<li>  The path by which the vaccine product is taken into the body needs to be known.</li>
<li>  The quantity of vaccine product that was administered is needed.</li>
</ul>

### Steps to follow

We will create a derived profile of the applicable profile as defined in the [US Core implementation guide][1] to ensure compatibility. Creating a derived profile can either by downloading and saving the base profile or by installing the US Core FHIR package. Let's install US Core. 

1. Select your profiling folder in Forge and go to the dependencies tab.
2. Click on the Simplifier icon to search for packages in Simplifier.net
3. Search for `US` or `hl7.fhir.us.core` and install the '4.1.0' version by selecting it and clicking on 'Add'.
4. Navigate back to the project tab (and notice that the US core packages and their dependencies are shown), open the US core package, and navigate to the FHIR profile needed for this use case.
5. Right-click, and select 'New Derived Profile'
6. Provide the profile with metadata and notice that you have inherited all the constraints from the base profile in the element tree view.
7. Now, let's profile the use case requirements! 


[1]: https://www.hl7.org/fhir/us/core/ "HL7 FHIR® US Core Implementation Guide"



<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse5">Results after completing step 5</a>
      </h2>
    </div>
    <div id="collapse5" class="panel-collapse collapse">
      <div class="panel-body">
        <p><b>Differential view of 'Hospital X Immunization step 5'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXImmunization-Step5, diff}}  </p>
        <p>               
  </div>
</div>