---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	subject : "Did you see last night's game?",
	importance : Importance.Low,
	body : {
		contentType : BodyType.HTML,
		content : "They were <b>awesome</b>!",
	},
	toRecipients : [
		{
			emailAddress : {
				address : "AdeleV@contoso.onmicrosoft.com",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```