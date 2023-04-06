---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrintTaskDefinition = {
	displayName : "Test TaskDefinitionName",
	createdBy : {
		displayName : "Requesting App Display Name",
	},
};

const result = async () => {
	await graphServiceClient.print.taskDefinitionsById("printTaskDefinition-id").patch(requestBody);
}


```