---
topic: Validationbonus2
---
# Step 8: Validation (bonus) ✔️

<ul class="roundbox">
<p>The developers of the general practitioners that will send patient data to Hospital X are starting to implement the use case based on your profiles. They are missing examples of resources that conform to the FHIR profiles of Hospital X.</p>

<li> Provide valid instances of the published profiles to demonstrate the expected FHIR resources.</li>
<li> Test the profiles by validating the example instances against the profiles. </li>
</ul>

### Steps to follow
1. It is good practice to create an instance of your profile while creating that profile. It will improve your modeling, provide documentation for the implementers and allow you to validate and test your profile. Therefore, the bonus exercise is to create instances that conform to the built profiles.
2. Upload the instances to your project. Or move on to step #5.
3. Make sure the instance has a `.meta.profile` element that includes the canonical URL of your profile.
4. Navigate to the instance in your Simplifier project and hit the validate icon in the top right. 
Note: if you are on a paid plan, you can run the Quality Control feature validating the entire project in one go!
5. Instead of uploading the instance, you can also copy and paste it in [simplifier/validate][1]. Make sure R4 is selected and you scope the validation to your project/package.
6. If you want to know all the benefits of publishing and validating your profiles with packages, the following exercises are highly recommended: [ACME R4 Package Tutorial][2]. 


[1]: https://simplifier.net/validate "Simplifier Validator"
[2]: https://simplifier.net/guide/acme-r4-packages-tutorial "Package Tutorial"
