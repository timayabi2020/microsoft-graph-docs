---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UrlThreatSubmission = {
	"@odata.type" : "#microsoft.graph.urlThreatSubmission",
	category : SubmissionCategory.Phishing,
	webUrl : "http://phishing.contoso.com",
};

const result = async () => {
	await graphServiceClient.security.threatSubmission.urlThreats.post(requestBody);
}


```