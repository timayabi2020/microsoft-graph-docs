---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageResourceRequest = {
	catalogId : "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
	requestType : "AdminAdd",
	justification : "",
	accessPackageResource : {
		displayName : "Marketing resources",
		description : "Marketing group",
		resourceType : "AadGroup",
		originId : "e93e24d1-2b65-4a6c-a1dd-654a12225487",
		originSystem : "AadGroup",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```