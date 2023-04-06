---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	displayName : "extension-policy",
	description : "test",
	accessPackageId : "ba5807c7-2aa9-4c8a-907e-4a17ee587500",
	canExtend : false,
	requestApprovalSettings : null,
	requestorSettings : {
		acceptRequests : true,
		scopeType : "AllExistingDirectorySubjects",
		allowedRequestors : [
		],
		additionalData : {
			isOnBehalfAllowed : false,
		},
	},
	accessReviewSettings : null,
	questions : [
	],
	customExtensionHandlers : [
		{
			stage : AccessPackageCustomExtensionStage.AssignmentRequestCreated,
			customExtension : {
				id : "219f57b6-7983-45a1-be01-2c228b7a43f8",
			},
		},
		{
			stage : AccessPackageCustomExtensionStage.AssignmentRequestGranted,
			customExtension : {
				id : "219f57b6-7983-45a1-be01-2c228b7a43f8",
			},
		},
	],
	additionalData : {
		expiration : {
			type : "afterDuration",
			duration : "P365D",
		},
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(requestBody);
}


```