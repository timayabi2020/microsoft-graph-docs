---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PublishPostRequestBody = {
	revision : "1.0",
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteListsById("browserSiteList-id").publish.post(requestBody);
}


```