---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		identity : {
			additionalData : {
				phone : {
					"@odata.type" : "#microsoft.graph.identity",
					id : "+12345678901",
				},
			},
		},
		additionalData : {
			"endpointType" : "default",
			"languageId" : "languageId-value",
			"region" : "region-value",
		},
	},
	additionalData : {
		"clientContext" : "9e90d1c1-f61e-43e7-9f75-d420159aae08",
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```