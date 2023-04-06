---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UploadPkcs12PostRequestBody = {
	key : "Base64-encoded-pfx-content",
	password : "password-value",
};

const result = async () => {
	await graphServiceClient.trustFramework.keySetsById("trustFrameworkKeySet-id").uploadPkcs12.post(requestBody);
}


```