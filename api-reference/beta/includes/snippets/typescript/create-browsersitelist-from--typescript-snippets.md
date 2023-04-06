---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BrowserSiteList = {
	displayName : "Production Site List A",
	description : "Production site list for team A",
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteLists.post(requestBody);
}


```