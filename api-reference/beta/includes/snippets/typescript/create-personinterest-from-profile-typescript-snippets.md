---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonInterest = {
	categories : [
		"Sports",
	],
	description : "World's greatest football club",
	displayName : "Chelsea FC",
	webUrl : "https://www.chelseafc.com",
};

const result = async () => {
	await graphServiceClient.me.profile.interests.post(requestBody);
}


```