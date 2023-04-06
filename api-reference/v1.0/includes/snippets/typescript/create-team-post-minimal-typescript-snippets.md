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
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')",
			},
		},
	],
	additionalData : {
		"template@odata.bind" : "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
	},
};

const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```