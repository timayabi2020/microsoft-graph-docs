---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleAssignmentScheduleRequest = {
	action : "AdminAssign",
	justification : "Assign User Admin to IT Helpdesk (User) group",
	roleDefinitionId : "fdd7a751-b60b-444a-984c-02652fe8fa1c",
	directoryScopeId : "/",
	principalId : "07706ff1-46c7-4847-ae33-3003830675a1",
	scheduleInfo : {
		startDateTime : new Date("2021-07-01T00:00:00Z"),
		expiration : {
			type : ExpirationPatternType.NoExpiration,
		},
	},
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignmentScheduleRequests.post(requestBody);
}


```