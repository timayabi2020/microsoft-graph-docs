---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentRequest = {
	requestType : "AdminAdd",
	accessPackageAssignment : {
		target : {
			email : "user@contoso.com",
		},
		assignmentPolicyId : "2264bf65-76ba-417b-a27d-54d291f0cbc8",
		accessPackageId : "a914b616-e04e-476b-aa37-91038f0b165b",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(requestBody);
}


```