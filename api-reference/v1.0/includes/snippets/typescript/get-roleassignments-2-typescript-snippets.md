---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: " principalId eq '5bde3e51-d13b-4db1-9948-fe4b109d11a7'",
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.get(configuration);
}


```