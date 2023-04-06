---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Chat = {
	chatType : ChatType.Group,
	topic : "Group chat title",
	members : [
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"guest",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g')",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```