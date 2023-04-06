---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleDefinition = {
	description : "An example custom role",
	displayName : "ExampleCustomRole",
	rolePermissions : [
		{
			allowedResourceActions : [
				"Microsoft.CloudPC/CloudPCs/Read",
			],
		},
	],
	additionalData : {
		"condition" : "null",
	},
};

const result = async () => {
	await graphServiceClient.roleManagement.cloudPC.roleDefinitions.post(requestBody);
}


```