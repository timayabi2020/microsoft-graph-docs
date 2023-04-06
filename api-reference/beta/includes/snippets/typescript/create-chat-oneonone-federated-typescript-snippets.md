---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Chat = {
	chatType : ChatType.OneOnOne,
	members : [
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')",
				"tenantId" : "4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```