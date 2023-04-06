---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationSchool = {
	"@odata.type" : "#microsoft.graph.educationSchool",
	displayName : "String",
	description : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	principalEmail : "String",
	principalName : "String",
	externalPrincipalId : "String",
	lowestGrade : "String",
	highestGrade : "String",
	schoolNumber : "String",
	externalId : "String",
	phone : "String",
	fax : "String",
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	address : {
		"@odata.type" : "microsoft.graph.physicalAddress",
	},
};

const result = async () => {
	await graphServiceClient.education.schools.post(requestBody);
}


```