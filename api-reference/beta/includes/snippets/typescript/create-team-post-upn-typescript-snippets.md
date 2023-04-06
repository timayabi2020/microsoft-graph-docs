---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Team = {
	displayName : "My Sample Team",
	description : "My Sample Team’s Description",
	members : [
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
			},
		},
	],
	additionalData : {
		"template@odata.bind" : "https://graph.microsoft.com/beta/teamsTemplates('standard')",
	},
};

const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```