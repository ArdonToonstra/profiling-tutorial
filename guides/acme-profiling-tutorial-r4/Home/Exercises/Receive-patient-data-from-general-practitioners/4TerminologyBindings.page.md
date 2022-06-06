---
topic: Terminologybindings
---
# Step 4: Terminology bindings 💎

<ul class="roundbox">
<p>Hospital X can only handle certain terminology and wants to capture specific data on the conditions that the patients have. The following requirements are specified:</p>
<li> The conditions need to have coded information that is the identification of the condition. </li>
<li> The hospital wants to register conditions with SNOMED CT codes and only allows ‘Clinical Finding’ codes. </li>
</ul>

### Steps to follow
1. Find the right FHIR ValueSet that matches the above-described needs for the Condition resource. You can, for example, search in the [FHIR Registry][1], [Simplifier.net][2] or the [list of ValueSet in the core FHIR specification][3]. **Shortcut** : link to the [SNOMEDCTClinicalFindings][4] ValueSet.
2. Bind the ValueSet to the correct element in the profile. 
3. Adjust the binding strength to _required_.
4. Make the element mandatory.

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse4">Results after completing step 4</a>
      </h2>
    </div>
    <div id="collapse4" class="panel-collapse collapse">
      <div class="panel-body">
        <p><b>Differential view of 'Hospital X Condition step 4'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXCondition-Step4, diff}}  </p>
        <p>               
  </div>
</div>



[1]: https://registry.fhir.org/ "HL7 FHIR registry"
[2]: https://simplifier.net/search?fhirVersion=R4 "Simplifier registry"
[3]: http://hl7.org/fhir/R4/terminologies-valuesets.html "HL7 FHIR Core ValueSet reistry"
[4]: https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/83436/~overview
[5]: http://hl7.org/fhir/ValueSet/research-subject-status "ResearchSubjectStatus"
