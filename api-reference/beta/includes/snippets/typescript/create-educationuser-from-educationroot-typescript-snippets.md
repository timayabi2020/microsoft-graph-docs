---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationUser = {
	displayName : "Dion Matheson",
	givenName : "Dion",
	middleName : null,
	surname : "Matheson",
	mail : "DionM@contoso.com",
	mobilePhone : "+1 (253) 555-0101",
	createdBy : {
		user : {
			displayName : "Susana Rocha",
			id : "14012",
		},
	},
	externalSource : EducationExternalSource.Sis,
	mailingAddress : {
		city : "Los Angeles",
		countryOrRegion : "United States",
		postalCode : "98055",
		state : "CA",
		street : "12345 Main St.",
	},
	primaryRole : EducationUserRole.Student,
	residenceAddress : {
		city : "Los Angeles",
		countryOrRegion : "United States",
		postalCode : "98055",
		state : "CA",
		street : "12345 Main St.",
	},
};

const result = async () => {
	await graphServiceClient.education.users.post(requestBody);
}


```