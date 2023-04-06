---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GovernanceRoleAssignmentRequest = {
	roleDefinitionId : "70521f3e-3b95-4e51-b4d2-a2f485b02103",
	resourceId : "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
	subjectId : "1566d11d-d2b6-444a-a8de-28698682c445",
	assignmentState : "Eligible",
	type : "AdminUpdate",
	schedule : {
		type : "Once",
		startDateTime : new Date("2018-03-08T05:42:45.317Z"),
		endDateTime : new Date("2018-06-05T05:42:31.000Z"),
	},
};

const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleAssignmentRequests.post(requestBody);
}


```