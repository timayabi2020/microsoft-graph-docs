---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcExternalPartnerSetting = {
	"@odata.type" : "#microsoft.graph.cloudPcExternalPartnerSetting",
	partnerId : "198d7140-80bb-4843-8cc4-811377a49a92",
	enableConnection : true,
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.externalPartnerSettings.post(requestBody);
}


```