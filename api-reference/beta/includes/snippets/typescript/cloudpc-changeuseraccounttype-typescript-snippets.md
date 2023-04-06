---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChangeUserAccountTypePostRequestBody = {
	userAccountType : CloudPcUserAccountType.Administrator,
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.cloudPCsById("cloudPC-id").changeUserAccountType.post(requestBody);
}


```