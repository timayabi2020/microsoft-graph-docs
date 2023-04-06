---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LegalHold = {
	"@odata.type" : "#microsoft.graph.ediscovery.legalHold",
	description : "String",
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	isEnabled : boolean,
	status : LegalHoldStatus.String,
	contentQuery : "String",
	errors : [
		"String",
	],
	displayName : "String",
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").legalHolds.post(requestBody);
}


```