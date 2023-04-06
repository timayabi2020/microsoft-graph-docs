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
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('alex@contoso.com')",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```