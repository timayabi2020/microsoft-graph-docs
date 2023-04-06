---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UpdateAdDomainPasswordPostRequestBody = {
	adDomainPassword : "AdDomainPassword value",
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.onPremisesConnectionsById("cloudPcOnPremisesConnection-id").updateAdDomainPassword.post(requestBody);
}


```