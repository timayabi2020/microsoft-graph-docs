---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InferenceClassificationOverride = {
	classifyAs : InferenceClassificationType.Focused,
};

const result = async () => {
	await graphServiceClient.me.inferenceClassification.overridesById("inferenceClassificationOverride-id").patch(requestBody);
}


```