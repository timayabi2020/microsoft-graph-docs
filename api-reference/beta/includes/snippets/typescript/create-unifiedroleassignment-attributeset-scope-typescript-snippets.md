---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleAssignment = {
	"@odata.type" : "#microsoft.graph.unifiedRoleAssignment",
	roleDefinitionId : "58a13ea3-c632-46ae-9ee0-9c0d43cd7f3d",
	principalId : "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
	directoryScopeId : "/attributeSets/Engineering",
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.post(requestBody);
}


```