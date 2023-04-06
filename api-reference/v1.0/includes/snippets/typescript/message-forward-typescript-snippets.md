---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ForwardPostRequestBody = {
	comment : "comment-value",
	toRecipients : [
		{
			emailAddress : {
				name : "name-value",
				address : "address-value",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").forward.post(requestBody);
}


```