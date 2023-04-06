---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	accessPackageId : "88203d16-0e31-41d4-87b2-dd402f1435e9",
	displayName : "Specific users",
	description : "Specific users can request assignment",
	accessReviewSettings : null,
	durationInDays : 30,
	requestorSettings : {
		scopeType : "SpecificDirectorySubjects",
		acceptRequests : true,
		allowedRequestors : [
			{
				"@odata.type" : "#microsoft.graph.singleUser",
				isBackup : false,
				additionalData : {
					"id" : "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
					"description" : "Requestor1",
				},
			},
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