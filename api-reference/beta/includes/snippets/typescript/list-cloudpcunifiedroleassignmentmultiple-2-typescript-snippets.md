---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.cloudPC.roleAssignments.get(configuration);
}


```