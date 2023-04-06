---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.get(configuration);
}


```