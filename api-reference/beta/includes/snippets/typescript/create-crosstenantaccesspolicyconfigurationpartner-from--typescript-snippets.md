---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CrossTenantAccessPolicyConfigurationPartner = {
	tenantId : "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
	b2bDirectConnectOutbound : {
		usersAndGroups : {
			accessType : CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked,
			targets : [
				{
					target : "6f546279-4da5-4b53-a095-09ea0cef9971",
					targetType : CrossTenantAccessPolicyTargetType.Group,
				},
			],
		},
	},
	b2bDirectConnectInbound : {
		applications : {
			accessType : CrossTenantAccessPolicyTargetConfigurationAccessType.Allowed,
			targets : [
				{
					target : "Office365",
					targetType : CrossTenantAccessPolicyTargetType.Application,
				},
			],
		},
	},
};

const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.partners.post(requestBody);
}


```