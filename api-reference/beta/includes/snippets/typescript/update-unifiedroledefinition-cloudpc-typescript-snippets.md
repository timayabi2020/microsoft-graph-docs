---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleDefinition = {
	description : "Update basic properties and permission of application registrations",
	displayName : "ExampleCustomRole",
	rolePermissions : [
		{
			allowedResourceActions : [
				"Microsoft.CloudPC/CloudPCs/Read",
				"Microsoft.CloudPC/CloudPCs/Reprovision",
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.roleManagement.cloudPC.roleDefinitionsById("unifiedRoleDefinition-id").patch(requestBody);
}


```