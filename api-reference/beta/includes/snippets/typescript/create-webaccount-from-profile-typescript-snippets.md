---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WebAccount = {
	description : "My Github contributions!",
	userId : "innocenty.popov",
	service : {
		name : "GitHub",
		webUrl : "https://github.com",
	},
};

const result = async () => {
	await graphServiceClient.me.profile.webAccounts.post(requestBody);
}


```