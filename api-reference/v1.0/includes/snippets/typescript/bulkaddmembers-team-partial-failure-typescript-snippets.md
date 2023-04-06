---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddPostRequestBody = {
	values : [
		{
			"@odata.type" : "microsoft.graph.aadUserConversationMember",
			roles : [
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')",
			},
		},
		{
			"@odata.type" : "microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").members.add.post(requestBody);
}


```