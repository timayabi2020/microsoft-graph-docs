---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"User-Agent": "ContosoLOBApp/1.0",
	}
};
const requestBody : EvaluateClassificationResultsPostRequestBody = {
	contentInfo : {
		"@odata.type" : "#microsoft.graph.contentInfo",
		format : ContentFormat.Default,
		identifier : null,
		state : ContentState.Rest,
		additionalData : {
			"format@odata.type" : "#microsoft.graph.contentFormat",
			"state@odata.type" : "#microsoft.graph.contentState",
		},
	},
	classificationResults : [
		{
			sensitiveTypeId : "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
			count : 4,
			confidenceLevel : 75,
		},
	],
};

const result = async () => {
	await graphServiceClient.informationProtection.policy.labels.evaluateClassificationResults.post(requestBody, configuration);
}


```