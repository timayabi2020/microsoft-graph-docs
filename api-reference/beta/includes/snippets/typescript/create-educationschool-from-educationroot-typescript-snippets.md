---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationSchool = {
	displayName : "Fabrikam High School",
	description : "Magnate school for the arts. Los Angeles School District",
	externalSource : EducationExternalSource.String,
	principalEmail : "AmyR@fabrikam.com",
	principalName : "Amy Roebuck",
	externalPrincipalId : "14007",
	highestGrade : "12",
	lowestGrade : "9",
	schoolNumber : "10002",
	address : {
		city : "Los Angeles",
		countryOrRegion : "United States",
		postalCode : "98055",
		state : "CA",
		street : "12345 Main St.",
	},
	externalId : "10002",
	phone : "+1 (253) 555-0102",
};

const result = async () => {
	await graphServiceClient.education.schools.post(requestBody);
}


```