---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'",
		expand: ["target","accessPackageAssignmentResourceRoles"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignments.get(configuration);
}


```