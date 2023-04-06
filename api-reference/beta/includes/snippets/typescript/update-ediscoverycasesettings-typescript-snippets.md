---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryCaseSettings = {
	"@odata.type" : "#microsoft.graph.security.ediscoveryCaseSettings",
	redundancyDetection : {
		"@odata.type" : "microsoft.graph.security.redundancyDetectionSettings",
	},
	topicModeling : {
		"@odata.type" : "microsoft.graph.security.topicModelingSettings",
	},
	ocr : {
		"@odata.type" : "microsoft.graph.security.ocrSettings",
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").settings.patch(requestBody);
}


```