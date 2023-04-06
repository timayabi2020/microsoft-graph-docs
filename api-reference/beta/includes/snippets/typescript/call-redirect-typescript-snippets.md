---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RedirectPostRequestBody = {
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
	callbackUri : "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").redirect.post(requestBody);
}


```