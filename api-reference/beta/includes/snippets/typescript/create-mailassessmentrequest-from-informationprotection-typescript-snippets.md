---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ThreatAssessmentRequest = {
	"@odata.type" : "#microsoft.graph.mailAssessmentRequest",
	expectedAssessment : ThreatExpectedAssessment.Block,
	category : ThreatCategory.Spam,
	additionalData : {
		"recipientEmail" : "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
		"messageUri" : "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
	},
};

const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequests.post(requestBody);
}


```