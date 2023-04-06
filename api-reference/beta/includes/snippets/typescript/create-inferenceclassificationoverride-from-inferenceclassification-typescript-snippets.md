---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InferenceClassificationOverride = {
	classifyAs : InferenceClassificationType.Focused,
	senderEmailAddress : {
		name : "Samantha Booth",
		address : "samanthab@adatum.onmicrosoft.com",
	},
};

const result = async () => {
	await graphServiceClient.me.inferenceClassification.overrides.post(requestBody);
}


```