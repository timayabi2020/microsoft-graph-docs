---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GovernanceRoleAssignmentRequest = {
	roleDefinitionId : "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
	resourceId : "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
	subjectId : "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
	assignmentState : "Eligible",
	type : "AdminAdd",
	reason : "Assign an eligible role",
	schedule : {
		startDateTime : new Date("2018-05-12T23:37:43.356Z"),
		endDateTime : new Date("2018-11-08T23:37:43.356Z"),
		type : "Once",
	},
};

const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleAssignmentRequests.post(requestBody);
}


```