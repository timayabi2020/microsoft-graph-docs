---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["effectiveRules","rules"],
	}
};

const result = async () => {
	await graphServiceClient.policies.roleManagementPoliciesById("unifiedRoleManagementPolicy-id").get(configuration);
}


```