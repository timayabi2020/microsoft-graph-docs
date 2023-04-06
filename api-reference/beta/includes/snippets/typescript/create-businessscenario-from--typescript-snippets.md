---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BusinessScenario = {
	"@odata.type" : "#microsoft.graph.businessScenario",
	displayName : "Contoso Order Tracking",
	uniqueName : "com.contoso.apps.ordertracking",
};

const result = async () => {
	await graphServiceClient.solutions.businessScenarios.post(requestBody);
}


```