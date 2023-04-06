---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TransferPostRequestBody = {
	transferTarget : {
		"@odata.type" : "#microsoft.graph.invitationParticipantInfo",
		endpointType : EndpointType.Default,
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
			"languageId" : "en-us",
			"region" : "amer",
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```