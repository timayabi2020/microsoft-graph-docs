---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Conversation = {
	topic : "Take your wellness days and rest",
	threads : [
		{
			posts : [
				{
					body : {
						contentType : BodyType.Html,
						content : "Contoso cares about you: Rest and Recharge",
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