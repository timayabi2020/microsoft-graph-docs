---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrivilegedRoleAssignment = {
	userId : "userId-value",
	roleId : "roleId-value",
};

const result = async () => {
	await graphServiceClient.privilegedRoleAssignments.post(requestBody);
}


```