---
topic: Extensions2
---
# Step 2: Extensions ➕

<ul class="roundbox">
<p>Hospital X wants to capture additional data on the patient, which is not represented in the base resource. The following (additional) requirements are specified:</p>
<li> Place of birth is mandatory. </li>
<li> Optional information on inclusion in one or more clinical studies. </li>
</ul>


### Steps to follow
##### Simple extension
1.  Find a relevant extension for place of birth. You can, for example, search in the [FHIR Registry][1], [Simplifier.net][2] or the [list of extensions in the core FHIR specification][3].
2. Found one? 
   - Download the extension as XML or JSON and save it in your project folder. You need to refresh the folder in Forge to see it.
   - Or... if you know which package contains the desired FHIR resource installing the package may even be more straightforward. 
      - In Forge: go to the dependencies tab
      - Go to Simplifier icon 
      - Search for `hl7.fhir.r4.core`
      - Install version 4.0.1 by selecting it and clicking on ‘Add’

3. Add the extension to the patient profile, provide an appropriate extension slice name and make it mandatory.

##### Complex extension
**Note:** This does not concern a real-world example (instead of an extension, the `ResearchSubject` resource could be used). Creating this extension solely demonstrates how a (complex) extension can be created. 

1. Create a new extension for clinical study inclusion by selecting the profiling folder in Forge and clicking 'New Extension'. Select 'Extension definition' in the left menu and use the 'profiles-types.xml' in the new screen that pops up.
2. The extension needs a canonical URL as well, and it needs to contain the context where this extension is allowed to be used. You can set this in the 'Properties' tab of the extension. (Context Type = 'fhirpath' and Context Expression = 'Patient')
3. Add three elements: clinical trial number (Identifier), period of involvement (Period), and inclusion status (CodeableConcept).
5. Add the extension to your patient profile.

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h2 class="panel-title">
        <a data-toggle="collapse" href="#collapse2">Results after completing step 2</a>
      </h2>
    </div>
    <div id="collapse2" class="panel-collapse collapse">
      <div class="panel-body">
        <b>Differential view of 'Hospital X Patient Step 2'</b>
            {{render:http://ardon.nl/fhir/StructureDefinition/HospitalXPatient-Step2, diff}}     
                <b>Differential view of the extension 'Hospital X Patient InclusionStatus step 2'</b>
            {{render:http://ardon.nl/fhir/StructureDefinition/InclusionStatus-Step2, diff}}               
  </div>
</div>



[1]: https://registry.fhir.org/ "HL7 FHIR registry"
[2]: https://simplifier.net/search?fhirVersion=R4 "Simplifier registry"
[3]: http://hl7.org/fhir/R4/extensibility-registry.html "HL7 FHIR Core extension reistry"
[4]: https://www.hl7.org/fhir/R4/valueset-research-subject-status.html "ResearchSubjectStatus ValueSet"