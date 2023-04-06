---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkforceIntegration = {
	displayName : "displayName-value",
	apiVersion : 99,
	encryption : {
		protocol : WorkforceIntegrationEncryptionProtocol.Protocol-value,
		secret : "secret-value",
	},
	isActive : true,
	url : "url-value",
	supportedEntities : WorkforceIntegrationSupportedEntities.SupportedEntities-value,
};

const result = async () => {
	await graphServiceClient.teamwork.workforceIntegrationsById("workforceIntegration-id").patch(requestBody);
}


```