---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"X-MS-CloudPC-USGovCloudTenantAADToken": "{token}",
	}
};
const requestBody : CrossCloudGovernmentOrganizationMappingPostRequestBody = {
};

async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.crossCloudGovernmentOrganizationMapping.post(requestBody, configuration);
}


```