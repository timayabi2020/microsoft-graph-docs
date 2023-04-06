---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SynchronizationSecretKeyStringValuePair = {
	additionalData : {
		value : [
			{
				key : "BaseAddress",
				value : "user@domain.com",
			},
			{
				key : "SecretToken",
				value : "password-value",
			},
			{
				key : "SyncNotificationSettings",
				value : "{\"Enabled\":false,\"DeleteThresholdEnabled\":false}",
			},
			{
				key : "SyncAll",
				value : "false",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.secrets.put(requestBody);
}


```