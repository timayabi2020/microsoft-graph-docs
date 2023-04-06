---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackagesById("accessPackage-id").get(configuration);
}


```