---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	accountEnabled : true,
	displayName : "Requestor1",
	mailNickname : "Requestor1",
	userPrincipalName : "Requestor1@contoso.onmicrosoft.com",
	passwordProfile : {
		forceChangePasswordNextSignIn : true,
		password : "Contoso1234",
	},
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```