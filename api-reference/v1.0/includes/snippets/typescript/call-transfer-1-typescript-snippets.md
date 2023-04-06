---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		identity : {
			user : {
				id : "550fae72-d251-43ec-868c-373732c2704f",
				displayName : "Heidi Steen",
			},
		},
		additionalData : {
			"endpointType" : "default",
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```