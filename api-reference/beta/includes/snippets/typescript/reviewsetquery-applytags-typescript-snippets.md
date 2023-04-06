---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ApplyTagsPostRequestBody = {
	tagsToAdd : [
		{
			id : "b4798d14-748d-468e-a1ec-96a2b1d49677",
		},
	],
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").reviewSetsById("reviewSet-id").queriesById("reviewSetQuery-id").ediscoveryApplyTags.post(requestBody);
}


```