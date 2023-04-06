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
				application : {
					"@odata.type" : "#microsoft.graph.identity",
					displayName : "test bot 2",
					id : "22bfd41f-550e-477d-8789-f6f7bd2a5e8b",
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