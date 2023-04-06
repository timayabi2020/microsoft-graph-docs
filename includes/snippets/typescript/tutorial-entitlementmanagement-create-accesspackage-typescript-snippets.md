---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackage = {
	catalogId : "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
	displayName : "Marketing Campaign",
	description : "Access to resources for the campaign",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackages.post(requestBody);
}


```