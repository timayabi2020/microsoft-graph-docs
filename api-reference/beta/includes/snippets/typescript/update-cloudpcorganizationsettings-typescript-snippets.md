---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcOrganizationSettings = {
	"@odata.type" : "#microsoft.graph.cloudPcOrganizationSettings",
	enableMEMAutoEnroll : true,
	osVersion : CloudPcOperatingSystem.Windows11,
	userAccountType : CloudPcUserAccountType.StandardUser,
	windowsSettings : {
		language : "en-US",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.organizationSettings.patch(requestBody);
}


```