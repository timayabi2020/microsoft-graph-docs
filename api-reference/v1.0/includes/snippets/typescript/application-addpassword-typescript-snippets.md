---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddPasswordPostRequestBody = {
	passwordCredential : {
		displayName : "Password friendly name",
	},
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").addPassword.post(requestBody);
}


```