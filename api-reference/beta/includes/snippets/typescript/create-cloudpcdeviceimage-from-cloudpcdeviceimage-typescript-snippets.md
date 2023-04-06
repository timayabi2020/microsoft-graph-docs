---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcDeviceImage = {
	"@odata.type" : "#microsoft.graph.cloudPcDeviceImage",
	displayName : "Display Name value",
	osBuildNumber : "OS Build Number value",
	operatingSystem : "Operating System value",
	version : "Version value",
	sourceImageResourceId : "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.deviceImages.post(requestBody);
}


```