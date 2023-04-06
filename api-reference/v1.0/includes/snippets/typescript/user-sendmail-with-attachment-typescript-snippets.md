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
					address : "meganb@contoso.onmicrosoft.com",
				},
			},
		],
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.fileAttachment",
				name : "attachment.txt",
				contentType : "text/plain",
				additionalData : {
					"contentBytes" : "SGVsbG8gV29ybGQh",
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```