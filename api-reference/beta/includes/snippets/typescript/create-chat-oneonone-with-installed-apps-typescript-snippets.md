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
				"user@odata.bind" : "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')",
			},
		},
	],
	installedApps : [
		{
			additionalData : {
				"teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```