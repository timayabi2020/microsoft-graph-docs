---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Library Assist",
	displayName : "Library Assist",
	groupTypes : [
		"Unified",
	],
	mailEnabled : true,
	mailNickname : "library-help",
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").patch(requestBody);
}


```