---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		token: "1230919asd190410jlka",
	}
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").items.delta().get(configuration);
}


```