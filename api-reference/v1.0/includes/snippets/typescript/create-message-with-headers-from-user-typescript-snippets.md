---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	subject : "9/8/2018: concert",
	body : {
		contentType : BodyType.HTML,
		content : "The group represents Washington.",
	},
	toRecipients : [
		{
			emailAddress : {
				address : "AlexW@contoso.OnMicrosoft.com",
			},
		},
	],
	internetMessageHeaders : [
		{
			name : "x-custom-header-group-name",
			value : "Washington",
		},
		{
			name : "x-custom-header-group-id",
			value : "WA001",
		},
	],
};

const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```