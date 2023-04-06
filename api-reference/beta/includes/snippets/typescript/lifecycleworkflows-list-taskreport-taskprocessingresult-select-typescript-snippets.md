---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["id","failureReason","processingStatus","subject","task"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").taskReportsById("taskReport-id").taskProcessingResults.get(configuration);
}


```