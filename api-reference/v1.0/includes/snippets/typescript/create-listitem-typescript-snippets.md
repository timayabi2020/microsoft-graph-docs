---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ListItem = {
	fields : {
		additionalData : {
			"title" : "Widget",
			"color" : "Purple",
			weight : 32,
		},
	},
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").items.post(requestBody);
}


```