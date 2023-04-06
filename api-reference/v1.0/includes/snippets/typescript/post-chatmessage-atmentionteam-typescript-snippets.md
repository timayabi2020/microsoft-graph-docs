---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	body : {
		contentType : BodyType.Html,
		content : "<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>",
	},
	mentions : [
		{
			id : 0,
			mentionText : "GraphTesting",
			mentioned : {
				conversation : {
					id : "68a3e365-f7d9-4a56-b499-24332a9cc572",
					displayName : "GraphTesting",
					conversationIdentityType : TeamworkConversationIdentityType.Team,
				},
			},
		},
	],
	reactions : [
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```