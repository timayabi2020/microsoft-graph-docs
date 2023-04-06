---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleEligibilityScheduleRequest = {
	action : UnifiedRoleScheduleRequestActions.AdminRemove,
	principalId : "e77cbb23-0ff2-4e18-819c-690f58269752",
	roleDefinitionId : "fe930be7-5e62-47db-91af-98c3a49a38b1",
	directoryScopeId : "/",
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```