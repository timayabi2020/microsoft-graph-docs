---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BusinessScenario = {
	ownerAppIds : [
		"44109254-4b2b-7a33-76ee-c890a167b295",
		"13eb9d8b-1d63-4153-9417-3a69ab200a78",
	],
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").patch(requestBody);
}


```