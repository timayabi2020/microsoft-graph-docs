---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["principalId","action","roleDefinitionId"],
		expand: ["roleDefinition","activatedUsing","principal","targetSchedule"],
	}
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignmentScheduleRequestsById("unifiedRoleAssignmentScheduleRequest-id").get(configuration);
}


```