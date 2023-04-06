---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "odata.maxpagesize=2",
	}
,	queryParameters : {
		select: ["displayName"],
	}
};

const result = async () => {
	await graphServiceClient.me.contactFoldersById("contactFolder-id").contacts.delta().get(configuration);
}


```