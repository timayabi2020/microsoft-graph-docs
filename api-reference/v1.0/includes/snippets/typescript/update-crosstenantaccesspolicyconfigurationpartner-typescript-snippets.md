---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CrossTenantAccessPolicyConfigurationPartner = {
	inboundTrust : {
		isMfaAccepted : true,
		isCompliantDeviceAccepted : true,
		isHybridAzureADJoinedDeviceAccepted : true,
	},
};

const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.partnersById("crossTenantAccessPolicyConfigurationPartner-tenantId").patch(requestBody);
}


```