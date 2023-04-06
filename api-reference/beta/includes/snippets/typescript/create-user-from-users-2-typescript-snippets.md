---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	accountEnabled : true,
	displayName : "Adele Vance",
	mailNickname : "AdeleV",
	userPrincipalName : "AdeleV@contoso.onmicrosoft.com",
	passwordProfile : {
		forceChangePasswordNextSignIn : true,
		password : "xWwvJ]6NMw+bWH-d",
	},
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```