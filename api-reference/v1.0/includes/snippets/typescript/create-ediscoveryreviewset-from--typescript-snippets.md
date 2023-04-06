---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryReviewSet = {
	displayName : "My review set 2",
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").reviewSets.post(requestBody);
}


```