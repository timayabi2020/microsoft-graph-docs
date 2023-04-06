---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddKeyPostRequestBody = {
	keyCredential : {
		type : "X509CertAndPassword",
		usage : "Sign",
		key : "mIIDYDCCAki...",
	},
	passwordCredential : {
		secretText : "MKTr0w1...",
	},
	proof : "eyJ0eXAiOiJ...",
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").addKey.post(requestBody);
}


```