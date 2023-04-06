---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CrossTenantAccessPolicyConfigurationDefault = {
	b2bCollaborationOutbound : {
		usersAndGroups : {
			accessType : CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
			targets : [
				{
					target : "0be493dc-cb56-4a53-936f-9cf64410b8b0",
					targetType : CrossTenantAccessPolicyTargetType.Group,
				},
			],
		},
		applications : {
			accessType : CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
			targets : [
				{
					target : "AllApplications",
					targetType : CrossTenantAccessPolicyTargetType.Application,
				},
			],
		},
	},
};

const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.default.patch(requestBody);
}


```