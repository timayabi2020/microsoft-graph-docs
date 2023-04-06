---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CustomAccessPackageWorkflowExtension = {
	additionalData : {
		"@odata.type" : "#microsoft.graph.customAccessPackageWorkflowExtension",
		"displayName" : "test_action_0124_email",
		"description" : "this is for graph testing only",
	},
};

async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").customAccessPackageWorkflowExtensionsById("customAccessPackageWorkflowExtension-id").put(requestBody);
}


```