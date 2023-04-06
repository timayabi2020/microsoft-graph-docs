---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	displayName : "New Policy",
	description : "policy for assignment",
	allowedTargetScope : AllowedTargetScope.NotSpecified,
	specificAllowedTargets : [
	],
	expiration : {
		endDateTime : null,
		duration : null,
		type : ExpirationPatternType.NoExpiration,
	},
	requestorSettings : {
		enableTargetsToSelfAddAccess : false,
		enableTargetsToSelfUpdateAccess : false,
		enableTargetsToSelfRemoveAccess : false,
		allowCustomAssignmentSchedule : true,
		enableOnBehalfRequestorsToAddAccess : false,
		enableOnBehalfRequestorsToUpdateAccess : false,
		enableOnBehalfRequestorsToRemoveAccess : false,
		onBehalfRequestors : [
		],
	},
	requestApprovalSettings : {
		isApprovalRequiredForAdd : false,
		isApprovalRequiredForUpdate : false,
		stages : [
		],
	},
	accessPackage : {
		id : "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentPolicies.post(requestBody);
}


```