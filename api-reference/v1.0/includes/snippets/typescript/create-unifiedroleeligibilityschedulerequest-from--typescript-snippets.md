---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleEligibilityScheduleRequest = {
	action : UnifiedRoleScheduleRequestActions.AdminAssign,
	justification : "Assign Attribute Assignment Admin eligibility to restricted user",
	roleDefinitionId : "8424c6f0-a189-499e-bbd0-26c1753c96d4",
	directoryScopeId : "/",
	principalId : "071cc716-8147-4397-a5ba-b2105951cc0b",
	scheduleInfo : {
		startDateTime : new Date("2022-04-10T00:00:00Z"),
		expiration : {
			type : ExpirationPatternType.AfterDateTime,
			endDateTime : new Date("2024-04-10T00:00:00Z"),
		},
	},
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```