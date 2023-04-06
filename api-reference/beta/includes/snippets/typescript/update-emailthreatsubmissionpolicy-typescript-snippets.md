---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EmailThreatSubmissionPolicy = {
	isReportToMicrosoftEnabled : false,
};

const result = async () => {
	await graphServiceClient.security.threatSubmission.emailThreatSubmissionPoliciesById("emailThreatSubmissionPolicy-id").patch(requestBody);
}


```