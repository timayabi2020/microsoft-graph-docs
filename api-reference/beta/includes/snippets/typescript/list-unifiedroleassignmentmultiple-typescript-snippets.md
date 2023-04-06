---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.deviceManagement.roleAssignments.get(configuration);
}


```