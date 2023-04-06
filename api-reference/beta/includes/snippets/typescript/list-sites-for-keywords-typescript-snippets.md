---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["siteCollection","webUrl"],
		filter: "siteCollection/root ne null",
	}
};

const result = async () => {
	await graphServiceClient.sites.get(configuration);
}


```