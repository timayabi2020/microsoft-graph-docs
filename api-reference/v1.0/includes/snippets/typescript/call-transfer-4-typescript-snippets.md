---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		"@odata.type" : "#microsoft.graph.invitationParticipantInfo",
		identity : {
			"@odata.type" : "#microsoft.graph.identitySet",
			additionalData : {
				phone : {
					"@odata.type" : "#microsoft.graph.identity",
					id : "+12345678901",
				},
			},
		},
		replacesCallId : "e5d39592-99bd-4db8-bca8-30fb894ec51d",
		additionalData : {
			"endpointType" : "default",
			"languageId" : "en-us",
			"region" : "amer",
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