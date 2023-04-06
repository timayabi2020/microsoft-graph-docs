---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	displayName : "My First Shared Channel",
	description : "This is my first shared channel",
	membershipType : ChannelMembershipType.Shared,
	members : [
		{
			"@odata.type" : "#microsoft.graph.aadUserConversationMember",
			roles : [
				"owner",
			],
			additionalData : {
				"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('7640023f-fe43-573f-9ff4-84a9efe4acd6')",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```