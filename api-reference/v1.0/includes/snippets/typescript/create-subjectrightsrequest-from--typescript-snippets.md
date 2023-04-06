---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SubjectRightsRequest = {
	type : SubjectRightsRequestType.Microsoft.graph.subjectRightsRequestType,
	dataSubjectType : DataSubjectType.Microsoft.graph.dataSubjectType,
	regulations : [
		"String",
	],
	displayName : "String",
	description : "String",
	internalDueDateTime : new Date("String (timestamp)"),
	dataSubject : {
		firstName : "String",
		lastName : "String",
		email : "String",
		residency : "String",
		additionalData : {
			"phoneNumber" : "String",
			"sSN" : "String",
		},
	},
};

const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequests.post(requestBody);
}


```