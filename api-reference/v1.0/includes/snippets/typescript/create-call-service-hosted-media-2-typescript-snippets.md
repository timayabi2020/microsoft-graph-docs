---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	"@odata.type" : "#microsoft.graph.call",
	callbackUri : "https://bot.contoso.com/callback",
	source : {
		"@odata.type" : "#microsoft.graph.participantInfo",
		identity : {
			"@odata.type" : "#microsoft.graph.identitySet",
			additionalData : {
				applicationInstance : {
					"@odata.type" : "#microsoft.graph.identity",
					displayName : "Calling Bot",
					id : "3d913abb-aec0-4964-8fa6-3c6850c4f278",
				},
			},
		},
		countryCode : null,
		endpointType : null,
		region : null,
		languageId : null,
	},
	targets : [
		{
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
		},
	],
	requestedModalities : [
		modality : Modality.Audio,
	],
	mediaConfig : {
		"@odata.type" : "#microsoft.graph.serviceHostedMediaConfig",
	},
	tenantId : "aa67bd4c-8475-432d-bd41-39f255720e0a",
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```