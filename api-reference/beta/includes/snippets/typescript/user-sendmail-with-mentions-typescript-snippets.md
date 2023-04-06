---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendMailPostRequestBody = {
	message : {
		subject : "Project kickoff",
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
	},
};

const result = async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```