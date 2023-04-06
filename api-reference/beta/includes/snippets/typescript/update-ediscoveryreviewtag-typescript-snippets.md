---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryReviewTag = {
	displayName : "My tag API 2",
	description : "Use Graph API to create tags (updated)",
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").tagsById("ediscoveryReviewTag-id").patch(requestBody);
}


```