---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	"@odata.type" : "#Microsoft.Graph.channel",
	membershipType : ChannelMembershipType.Private,
	displayName : "My First Private Channel",
	description : "This is my first private channels",
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
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```