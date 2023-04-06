---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CrossTenantIdentitySyncPolicyPartner = {
	userSyncInbound : {
		isSyncAllowed : true,
	},
};

const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.partnersById("crossTenantAccessPolicyConfigurationPartner-tenantId").identitySynchronization.patch(requestBody);
}


```