---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendMailPostRequestBody = {
	message : {
		subject : "Meet for lunch?",
		body : {
			contentType : BodyType.Text,
			content : "The new cafeteria is open.",
		},
		toRecipients : [
			{
				emailAddress : {
					address : "samanthab@contoso.onmicrosoft.com",
				},
			},
		],
		ccRecipients : [
			{
				emailAddress : {
					address : "danas@contoso.onmicrosoft.com",
				},
			},
		],
	},
	saveToSentItems : false,
};

const result = async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```