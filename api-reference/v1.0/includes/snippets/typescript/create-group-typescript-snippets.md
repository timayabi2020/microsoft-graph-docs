---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Self help community for library",
	displayName : "Library Assist",
	groupTypes : [
		"Unified",
	],
	mailEnabled : true,
	mailNickname : "library",
	securityEnabled : false,
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```