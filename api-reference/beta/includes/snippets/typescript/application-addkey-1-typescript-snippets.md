---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddKeyPostRequestBody = {
	keyCredential : {
		type : "AsymmetricX509Cert",
		usage : "Verify",
		key : "mIIDYDCCAki...",
	},
	passwordCredential : null,
	proof : "eyJ0eXAiOiJ...",
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").addKey.post(requestBody);
}


```