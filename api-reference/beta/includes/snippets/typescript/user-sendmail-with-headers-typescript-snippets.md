---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendMailPostRequestBody = {
	message : {
		subject : "9/9/2018: concert",
		body : {
			contentType : BodyType.HTML,
			content : "The group represents Nevada.",
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
				value : "Nevada",
			},
			{
				name : "x-custom-header-group-id",
				value : "NV001",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```