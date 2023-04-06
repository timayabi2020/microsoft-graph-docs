---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackage = {
	catalogId : "aa2f6514-3232-46e7-a08a-2411ad8d7128",
	displayName : "sales reps",
	description : "outside sales representatives",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackages.post(requestBody);
}


```