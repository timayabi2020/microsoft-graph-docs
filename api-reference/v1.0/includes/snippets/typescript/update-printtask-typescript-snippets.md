---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrintTask = {
	status : {
		state : PrintTaskProcessingState.Completed,
		description : "completed",
	},
};

const result = async () => {
	await graphServiceClient.print.taskDefinitionsById("printTaskDefinition-id").tasksById("printTask-id").patch(requestBody);
}


```