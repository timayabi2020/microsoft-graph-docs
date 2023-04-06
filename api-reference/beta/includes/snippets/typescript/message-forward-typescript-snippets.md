---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ForwardPostRequestBody = {
	message : {
		isDeliveryReceiptRequested : true,
		toRecipients : [
			{
				emailAddress : {
					address : "danas@contoso.onmicrosoft.com",
					name : "Dana Swope",
				},
			},
		],
	},
	comment : "Dana, just want to make sure you get this.",
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").forward.post(requestBody);
}


```