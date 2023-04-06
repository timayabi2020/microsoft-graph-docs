---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageCatalog = {
	displayName : "sales",
	description : "for employees working with sales and outside sales partners",
	state : AccessPackageCatalogState.Published,
	isExternallyVisible : true,
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.catalogs.post(requestBody);
}


```