---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Alert = {
	assignedTo : "secAdmin@contoso.onmicrosoft.com",
	classification : AlertClassification.TruePositive,
	determination : AlertDetermination.Malware,
	status : AlertStatus.InProgress,
};

const result = async () => {
	await graphServiceClient.security.alerts_v2ById("alert-id").patch(requestBody);
}


```