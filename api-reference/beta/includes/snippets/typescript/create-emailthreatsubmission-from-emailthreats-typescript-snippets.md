---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EmailThreatSubmission = {
	"@odata.type" : "#microsoft.graph.emailUrlThreatSubmission",
	category : SubmissionCategory.Spam,
	recipientEmailAddress : "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
	additionalData : {
		"messageUrl" : "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
	},
};

const result = async () => {
	await graphServiceClient.security.threatSubmission.emailThreats.post(requestBody);
}


```