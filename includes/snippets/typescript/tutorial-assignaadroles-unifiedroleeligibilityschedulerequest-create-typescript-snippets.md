---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleEligibilityScheduleRequest = {
	action : UnifiedRoleScheduleRequestActions.AdminAssign,
	justification : "Assign User Admin eligibility to IT Helpdesk (User) group",
	roleDefinitionId : "fe930be7-5e62-47db-91af-98c3a49a38b1",
	directoryScopeId : "/",
	principalId : "e77cbb23-0ff2-4e18-819c-690f58269752",
	scheduleInfo : {
		startDateTime : new Date("2021-07-01T00:00:00Z"),
		expiration : {
			endDateTime : new Date("2022-06-30T00:00:00Z"),
			type : ExpirationPatternType.AfterDateTime,
		},
	},
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```