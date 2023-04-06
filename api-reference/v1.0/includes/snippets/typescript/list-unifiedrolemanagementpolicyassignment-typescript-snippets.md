---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "scopeId eq '/' and scopeType eq 'Directory'",
	}
};

const result = async () => {
	await graphServiceClient.policies.roleManagementPolicyAssignments.get(configuration);
}


```