---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UploadSecretPostRequestBody = {
	use : "use-value",
	k : "application-secret-to-be-uploaded",
	nbf : 1508969811,
	exp : 1508973711,
};

const result = async () => {
	await graphServiceClient.trustFramework.keySetsById("trustFrameworkKeySet-id").uploadSecret.post(requestBody);
}


```