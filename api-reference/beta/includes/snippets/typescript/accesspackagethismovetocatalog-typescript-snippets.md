---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MoveToCatalogPostRequestBody = {
	catalogId : "3301434b-99bd-46be-923b-d762c30c8e8b",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackagesById("accessPackage-id").moveToCatalog.post(requestBody);
}


```