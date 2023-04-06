---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddToReviewSetPostRequestBody = {
	sourceCollection : {
		id : "1a9b4145d8f84e39bc45a7f68c5c5119",
	},
	additionalData : {
		"additionalData" : "linkedFiles",
	},
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").reviewSetsById("reviewSet-id").ediscoveryAddToReviewSet.post(requestBody);
}


```