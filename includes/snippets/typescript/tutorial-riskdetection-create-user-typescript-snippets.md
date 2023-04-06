---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	accountEnabled : true,
	displayName : "MyTestUser1",
	mailNickname : "MyTestUser1",
	userPrincipalName : "MyTestUser1@contoso.com",
	passwordProfile : {
		forceChangePasswordNextSignIn : true,
		password : "Contoso1234",
	},
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```