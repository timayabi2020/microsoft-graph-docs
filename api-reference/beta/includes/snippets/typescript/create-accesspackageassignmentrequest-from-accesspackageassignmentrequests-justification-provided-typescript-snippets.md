---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentRequest = {
	requestType : "UserAdd",
	accessPackageAssignment : {
		accessPackageId : "a914b616-e04e-476b-aa37-91038f0b165b",
	},
	justification : "Need access to New Hire access package",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(requestBody);
}


```