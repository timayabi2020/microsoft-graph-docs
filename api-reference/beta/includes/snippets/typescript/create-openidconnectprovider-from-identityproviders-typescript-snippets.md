---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityProvider = {
	"@odata.type" : "microsoft.graph.openIdConnectProvider",
	name : "Login with the Contoso identity provider",
	type : "OpenIDConnect",
	clientId : "56433757-cadd-4135-8431-2c9e3fd68ae8",
	clientSecret : "12345",
	additionalData : {
		claimsMapping : {
			userId : "myUserId",
			givenName : "myGivenName",
			surname : "mySurname",
			email : "myEmail",
			displayName : "myDisplayName",
		},
		"domainHint" : "mycustomoidc",
		"metadataUrl" : "https://mycustomoidc.com/.well-known/openid-configuration",
		"responseMode" : "form_post",
		"responseType" : "code",
		"scope" : "openid",
	},
};

const result = async () => {
	await graphServiceClient.identityProviders.post(requestBody);
}


```