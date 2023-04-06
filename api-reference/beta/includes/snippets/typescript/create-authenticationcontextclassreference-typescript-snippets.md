---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationContextClassReference = {
	id : "c1",
	displayName : "Contoso medium",
	description : "Medium protection level defined for Contoso policy",
	isAvailable : true,
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.authenticationContextClassReferences.post(requestBody);
}


```