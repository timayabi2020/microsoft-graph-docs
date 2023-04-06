---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddToReviewSetPostRequestBody = {
	search : {
		id : "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7",
	},
	additionalDataOptions : AdditionalDataOptions.LinkedFiles,
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").reviewSetsById("ediscoveryReviewSet-id").securityAddToReviewSet.post(requestBody);
}


```