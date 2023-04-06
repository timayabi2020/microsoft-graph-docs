---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	accessPackageId : "56ff43fd-6b05-48df-9634-956a777fce6d",
	displayName : "direct",
	description : "direct assignments by administrator",
	accessReviewSettings : null,
	requestorSettings : {
		scopeType : "NoSubjects",
		acceptRequests : true,
		allowedRequestors : [
		],
	},
	requestApprovalSettings : {
		isApprovalRequired : false,
		isApprovalRequiredForExtension : false,
		isRequestorJustificationRequired : false,
		approvalMode : "NoApproval",
		approvalStages : [
		],
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(requestBody);
}


```