---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryReviewTag = {
	displayName : "My tag API",
	description : "Use Graph API to create tags",
	childSelectability : ChildSelectability.Many,
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").tags.post(requestBody);
}


```