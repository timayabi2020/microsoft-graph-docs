---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InstantiatePostRequestBody = {
	displayName : "Azure AD SAML Toolkit",
};

const result = async () => {
	await graphServiceClient.applicationTemplatesById("applicationTemplate-id").instantiate.post(requestBody);
}


```