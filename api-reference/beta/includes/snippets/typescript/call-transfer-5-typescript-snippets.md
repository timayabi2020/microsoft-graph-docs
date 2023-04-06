---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		endpointType : EndpointType.Default,
		identity : {
			user : {
				id : "550fae72-d251-43ec-868c-373732c2704f",
				displayName : "Heidi Steen",
				additionalData : {
					"tenantId" : "72f988bf-86f1-41af-91ab-2d7cd011db47",
				},
			},
		},
	},
	transferee : {
		identity : {
			user : {
				id : "751f6800-3180-414d-bd94-333364659951",
				additionalData : {
					"tenantId" : "72f988bf-86f1-41af-91ab-2d7cd011db47",
				},
			},
		},
		participantId : "909c6581-5130-43e9-88f3-fcb3582cde37",
	},
	additionalData : {
		"languageId" : "languageId-value",
		"region" : "region-value",
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```