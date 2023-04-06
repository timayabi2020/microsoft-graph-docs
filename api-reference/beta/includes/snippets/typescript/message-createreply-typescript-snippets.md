---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CreateReplyPostRequestBody = {
	message : {
		toRecipients : [
			{
				emailAddress : {
					address : "samanthab@contoso.onmicrosoft.com",
					name : "Samantha Booth",
				},
			},
			{
				emailAddress : {
					address : "randiw@contoso.onmicrosoft.com",
					name : "Randi Welch",
				},
			},
		],
	},
	comment : "Samantha, Randi, would you name the group if the project is approved, please?",
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").createReply.post(requestBody);
}


```