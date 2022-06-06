---
topic: Slicing
---
# Step 6: Slicing ✂️🍕

<ul class="roundbox">
<p>Hospital X  has additional for the general practitioner data:</p>
<li> The general practitioner needs to have exactly one active (official) United States National Provider Identifier (NPI) identifier. </li>
<li> All other identifiers which are known for the practitioner, if any, also need to come from the NPI. But they need to be marked as ‘old’. </li>
</ul>

### Steps to follow
1. Open the previously created Practitioner profile.
2. Slice the `identifier` element and add two slices.
3. Define the slicing details on the sliced root. They are differentiated by the value of `identifier.use`.
4. Define the two slices representing the above requirements. The naming system for the NPI can be found at HL7's [known identifier systems][1].


<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse6">Results after completing step 6</a>
      </h2>
    </div>
    <div id="collapse6" class="panel-collapse collapse">
      <div class="panel-body">
        <p><b>Differential view of 'Hospital X Practitioner step 6'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXPractitioner-step6, diff}}  </p>
        <p>               
  </div>
</div>


[1]: https://www.hl7.org/fhir/identifier-registry.html "Known Identifier Systems "
