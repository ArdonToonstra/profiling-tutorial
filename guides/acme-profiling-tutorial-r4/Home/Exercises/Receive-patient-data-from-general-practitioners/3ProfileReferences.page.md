---
topic: Profilereferences2
---
# Step 3: Profile references

<ul class="roundbox">
<p>Hospital X wants to capture data on the conditions that the patients have and model this in FHIR. The following requirements are specified:</p>
<li> The condition has a link to the the earlier described patient model. </li>
<li> The general pracititioner who recorded the condition must be provided.</li>
<li> The hospital needs at least 1 identifier and 1 name (family and given) of the general practitioner for identification.</li> 
</ul>

### Steps to follow
1. Create a new profile based on the best FHIR resource to capture this information.
2. Make sure that the conditions can only refer to patients that conform to the profile we have defined in the previous exercise.
3. Create another profile based on the best FHIR resource to capture the general practitioner information.
4. Ensure that patient's conditions contain information on the recorder and that the recorder contains the required information described in the use case.


<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse3">Results after completing step 3</a>
      </h2>
    </div>
    <div id="collapse3" class="panel-collapse collapse">
      <div class="panel-body">
        <p><b>Differential view of 'Hospital X Condition step 3'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXCondition-Step3, diff}}  </p>
        <p>         
        <b>Differential view of 'Hospital X Practitioner step 3'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXPractitioner-Step3, diff}}    </p>            
  </div>
</div>
