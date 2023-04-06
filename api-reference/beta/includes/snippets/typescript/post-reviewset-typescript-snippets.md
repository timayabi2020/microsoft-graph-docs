---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReviewSet = {
	displayName : "My Reviewset 3",
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").reviewSets.post(requestBody);
}


```