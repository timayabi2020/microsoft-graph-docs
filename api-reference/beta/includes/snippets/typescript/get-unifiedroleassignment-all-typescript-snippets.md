---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"ConsistencyLevel": "eventual",
	}
,	queryParameters : {
		count: true,
		filter: "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.transitiveRoleAssignments.get(configuration);
}


```