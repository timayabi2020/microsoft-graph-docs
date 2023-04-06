---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ForwardPostRequestBody = {
	toRecipients : [
		{
			emailAddress : {
				address : "danas@contoso.onmicrosoft.com",
				name : "Dana Swope",
			},
		},
	],
	comment : "Dana, hope you can make this meeting.",
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").forward.post(requestBody);
}


```