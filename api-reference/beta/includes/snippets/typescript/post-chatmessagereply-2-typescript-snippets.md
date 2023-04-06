---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	createdDateTime : new Date("2019-02-04T19:58:15.511Z"),
	from : {
		user : {
			id : "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
			displayName : "John Doe",
		},
	},
	body : {
		contentType : BodyType.Html,
		content : "Hello World",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").replies.post(requestBody);
}


```