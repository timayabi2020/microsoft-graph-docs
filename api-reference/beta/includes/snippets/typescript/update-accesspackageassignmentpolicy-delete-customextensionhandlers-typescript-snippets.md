---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	id : "4540a08f-8ab5-43f6-a923-015275799197",
	displayName : "policy with custom access package workflow extension",
	description : "Run specified custom access package workflow extension at different stages.",
	accessPackageId : "ba5807c7-2aa9-4c8a-907e-4a17ee587500",
	requestApprovalSettings : null,
	requestorSettings : {
		acceptRequests : true,
		scopeType : "AllExistingDirectorySubjects",
		allowedRequestors : [
		],
	},
	accessReviewSettings : null,
	customExtensionHandlers : [
	],
	additionalData : {
		expiration : {
			type : "afterDuration",
			duration : "P365D",
		},
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPoliciesById("accessPackageAssignmentPolicy-id").put(requestBody);
}


```