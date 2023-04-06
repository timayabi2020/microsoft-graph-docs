---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Conversation = {
	topic : "New head count",
	threads : [
		{
			posts : [
				{
					body : {
						contentType : BodyType.Html,
						content : "The confirmation will come by the end of the week.",
					},
					newParticipants : [
						{
							emailAddress : {
								name : "Adele Vance",
								address : "AdeleV@contoso.onmicrosoft.com",
							},
						},
					],
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").conversations.post(requestBody);
}


```