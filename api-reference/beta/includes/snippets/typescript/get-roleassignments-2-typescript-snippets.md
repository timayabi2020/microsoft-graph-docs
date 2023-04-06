---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: " principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.get(configuration);
}


```