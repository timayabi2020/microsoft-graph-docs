---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleDefinition = {
	description : "Update basic properties of application registrations",
	displayName : "Application Registration Support Administrator",
	rolePermissions : [
		{
			allowedResourceActions : [
				"microsoft.directory/applications/basic/read",
			],
		},
	],
	isEnabled : true,
};

const result = async () => {
	await graphServiceClient.roleManagement.directory.roleDefinitions.post(requestBody);
}


```