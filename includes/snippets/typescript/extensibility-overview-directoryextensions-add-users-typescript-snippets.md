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
	userPrincipalName : "AdeleV@contoso.com",
	passwordProfile : {
		forceChangePasswordNextSignIn : false,
		password : "xWwvJ]6NMw+bWH-d",
	},
	additionalData : {
		"extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker" : "JobGroupN",
	},
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```