---
topic: BasicProfiling
---
# Step 1: Basic Profiling 🔥
<ul class="roundbox">
<p>Hospital X wants to receive patient data from general practitioners. The hospital has decided to build an interface conform the FHIR standard, starting with administrative data of patients. The following requirements are specified by Hosptial X:</p>
<li>	A patient has at least 1 name, and each name has at least 1 family name and 1 given name.</li>
<li>	Date of birth and gender are mandatory.</li>
<li>	A photo should not be allowed to be added.</li>
<li>	The hospital can only capture if a patient is deceased or not, not the actual dateTime.</li>
</ul>

### Steps to follow
1.	Create a new folder on your computer for this tutorial FHIR project.
2.	Start Forge and open the profile folder you just made.
3.	Create a new profile. Take a look at the [FHIR resource list][1]. In Forge, choose the resource that is the best fit for exchanging administrative patient data.
4.	Provide high-level metadata in the 'Properties' tab within Forge. Give it at least a name and a unique URL also named canonical, for example based on your name and country: 'http://**[yourname]**.**[yourcountrycode]**/fhir/StructureDefinition/HospitalXPatient'. For me that will be: `http://ardon.nl/fhir/StructureDefinition/HospitalXPatient`.
5.	Set the constraints according to the requirements of Hospital X in the 'Element Tree' view of Forge.

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse1">Results after completing step 1</a>
      </h2>
    </div>
    <div id="collapse1" class="panel-collapse collapse">
      <div class="panel-body">
      <b>Differential view of 'Hospital X Patient Step 1'</b>
            {{tree:http://ardon.nl/fhir/StructureDefinition/HospitalXPatient-Step1, diff}}            
  </div>
</div>

[1]: https://www.hl7.org/fhir/r4/resourcelist.html
[2]: https://simplifier.net/ui/project/create "Create a Simplifier project"
