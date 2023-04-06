---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackagesById("accessPackage-id").incompatibleAccessPackages.$ref.post(requestBody);
}


```