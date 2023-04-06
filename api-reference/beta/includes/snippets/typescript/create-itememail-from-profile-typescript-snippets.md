---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemEmail = {
	address : "Innocenty.Popov@adventureworks.com",
};

const result = async () => {
	await graphServiceClient.me.profile.emails.post(requestBody);
}


```