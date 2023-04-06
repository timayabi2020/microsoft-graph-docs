---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ApplyTagsPostRequestBody = {
	tagsToAdd : [
		{
			id : "d3d99dc704a74801b792b3e1e722aa0d",
		},
	],
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").reviewSetsById("ediscoveryReviewSet-id").queriesById("ediscoveryReviewSetQuery-id").securityApplyTags.post(requestBody);
}


```