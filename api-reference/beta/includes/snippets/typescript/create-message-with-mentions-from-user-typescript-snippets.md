---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	subject : "Party planning",
	toRecipients : [
		{
			emailAddress : {
				name : "Samantha Booth",
				address : "samanthab@contoso.onmicrosoft.com",
			},
		},
	],
	mentions : [
		{
			mentioned : {
				name : "Dana Swope",
				address : "danas@contoso.onmicrosoft.com",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```