---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageCatalog = {
	displayName : "Catalog One",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.catalogsById("accessPackageCatalog-id").patch(requestBody);
}


```