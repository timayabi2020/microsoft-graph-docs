---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'",
	}
};

const result = async () => {
	await graphServiceClient.identityProtection.riskDetections.get(configuration);
}


```