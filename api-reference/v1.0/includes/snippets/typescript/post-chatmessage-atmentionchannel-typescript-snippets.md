---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	body : {
		contentType : BodyType.Html,
		content : "<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>",
	},
	mentions : [
		{
			id : 0,
			mentionText : "General",
			mentioned : {
				conversation : {
					id : "19:0b50940236084d258c97b21bd01917b0@thread.skype",
					displayName : "General",
					conversationIdentityType : TeamworkConversationIdentityType.Channel,
				},
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```