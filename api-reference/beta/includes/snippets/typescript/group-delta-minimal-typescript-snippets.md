---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "return=minimal",
	}
,	queryParameters : {
		select: ["displayName","description","mailNickname"],
	}
};

const result = async () => {
	await graphServiceClient.groups.delta().get(configuration);
}


```