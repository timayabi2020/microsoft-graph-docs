---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConversationThread = {
	topic : "New Conversation Thread Topic",
	posts : [
		{
			body : {
				contentType : BodyType.Html,
				content : "this is body content",
			},
			newParticipants : [
				{
					emailAddress : {
						name : "Alex Darrow",
						address : "alexd@contoso.com",
					},
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threads.post(requestBody);
}


```