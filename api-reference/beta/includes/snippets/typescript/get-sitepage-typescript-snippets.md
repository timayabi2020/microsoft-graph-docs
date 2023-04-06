---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["id","title"],
		expand: ["webparts"],
	}
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").pagesById("sitePage-id").get(configuration);
}


```