---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ThreatAssessmentRequest = {
	"@odata.type" : "#microsoft.graph.fileAssessmentRequest",
	expectedAssessment : ThreatExpectedAssessment.Block,
	category : ThreatCategory.Malware,
	additionalData : {
		"fileName" : "test.txt",
		"contentData" : "VGhpcyBpcyBhIHRlc3QgZmlsZQ==",
	},
};

const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequests.post(requestBody);
}


```