---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Marketing group",
	displayName : "Marketing resources",
	mailEnabled : false,
	mailNickname : "markres",
	securityEnabled : true,
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```