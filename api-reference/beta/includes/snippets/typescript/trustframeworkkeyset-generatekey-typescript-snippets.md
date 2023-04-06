---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GenerateKeyPostRequestBody = {
	use : "sig",
	kty : "RSA",
	nbf : 1508969811,
	exp : 1508969811,
};

const result = async () => {
	await graphServiceClient.trustFramework.keySetsById("trustFrameworkKeySet-id").generateKey.post(requestBody);
}


```