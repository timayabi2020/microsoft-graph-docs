---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonName = {
	displayName : "Innocenty Popov",
	first : "Innocenty",
	initials : "IP",
	last : "Popov",
	languageTag : "en-US",
	maiden : null,
};

const result = async () => {
	await graphServiceClient.me.profile.names.post(requestBody);
}


```