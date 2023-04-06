---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcUserSetting = {
	"@odata.type" : "#microsoft.graph.cloudPcUserSetting",
	displayName : "Example",
	selfServiceEnabled : false,
	localAdminEnabled : true,
	restorePointSetting : {
		frequencyInHours : 16,
		userRestoreEnabled : true,
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.userSettings.post(requestBody);
}


```