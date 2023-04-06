---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoverySearch = {
	displayName : "Teams search",
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").searchesById("ediscoverySearch-id").patch(requestBody);
}


```