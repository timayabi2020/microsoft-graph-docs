---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationClass = {
	"@odata.type" : "#microsoft.graph.educationClass",
	displayName : "String",
	mailNickname : "String",
	description : "String",
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	classCode : "String",
	externalName : "String",
	externalId : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	grade : "String",
	term : {
		"@odata.type" : "microsoft.graph.educationTerm",
	},
};

const result = async () => {
	await graphServiceClient.education.classes.post(requestBody);
}


```