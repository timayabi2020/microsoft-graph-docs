---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CaseSettings = {
	redundancyDetection : {
		isEnabled : false,
		similarityThreshold : 70,
		minWords : 12,
		maxWords : 400000,
	},
	topicModeling : {
		isEnabled : false,
		ignoreNumbers : false,
		topicCount : 50,
		dynamicallyAdjustTopicCount : false,
	},
	ocr : {
		isEnabled : true,
		maxImageSize : 12000,
	},
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").settings.patch(requestBody);
}


```