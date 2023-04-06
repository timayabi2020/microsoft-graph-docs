---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	displayName : "John Smith",
	identities : [
		{
			signInType : "userName",
			issuer : "contoso.onmicrosoft.com",
			issuerAssignedId : "johnsmith",
		},
		{
			signInType : "emailAddress",
			issuer : "contoso.onmicrosoft.com",
			issuerAssignedId : "jsmith@yahoo.com",
		},
		{
			signInType : "federated",
			issuer : "facebook.com",
			issuerAssignedId : "5eecb0cd",
		},
	],
	passwordProfile : {
		password : "password-value",
		forceChangePasswordNextSignIn : false,
	},
	passwordPolicies : "DisablePasswordExpiration",
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```