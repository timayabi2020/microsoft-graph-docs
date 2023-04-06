---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentRequest = {
	requestType : AccessPackageRequestType.AdminRemove,
	assignment : {
		id : "a6bb6942-3ae1-4259-9908-0133aaee9377",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentRequests.post(requestBody);
}


```