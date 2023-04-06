---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcExternalPartnerSetting = {
	"@odata.type" : "#microsoft.graph.cloudPcExternalPartnerSetting",
	enableConnection : true,
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.externalPartnerSettingsById("cloudPcExternalPartnerSetting-id").patch(requestBody);
}


```