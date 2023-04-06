---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Incident = {
	classification : AlertClassification.TruePositive,
	determination : AlertDetermination.MultiStagedAttack,
	customTags : [
		"Demo",
	],
};

const result = async () => {
	await graphServiceClient.security.incidentsById("incident-id").patch(requestBody);
}


```