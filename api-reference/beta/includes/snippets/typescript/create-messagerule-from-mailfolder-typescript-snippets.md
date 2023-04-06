---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MessageRule = {
	displayName : "From partner",
	sequence : 2,
	isEnabled : true,
	conditions : {
		senderContains : [
			"adele",
		],
	},
	actions : {
		forwardTo : [
			{
				emailAddress : {
					name : "Alex Wilbur",
					address : "AlexW@contoso.onmicrosoft.com",
				},
			},
		],
		stopProcessingRules : true,
	},
};

const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messageRules.post(requestBody);
}


```