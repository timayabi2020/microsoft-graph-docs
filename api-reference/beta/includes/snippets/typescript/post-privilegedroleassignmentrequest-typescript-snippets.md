---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrivilegedRoleAssignmentRequest = {
	duration : "2",
	reason : "Activate the role for business purpose",
	ticketNumber : "234",
	ticketSystem : "system",
	schedule : {
		startDateTime : new Date("2018-02-08T02:35:17.903Z"),
	},
	type : "UserAdd",
	assignmentState : "Active",
	roleId : "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
};

const result = async () => {
	await graphServiceClient.privilegedRoleAssignmentRequests.post(requestBody);
}


```