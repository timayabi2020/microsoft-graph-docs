---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityApiConnector = {
	displayName : "Test API",
	targetUrl : "https://someotherapi.com/api",
	authenticationConfiguration : {
		"@odata.type" : "#microsoft.graph.pkcs12Certificate",
		additionalData : {
			"pkcs12Value" : "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
			"password" : "CertificatePassword",
		},
	},
};

const result = async () => {
	await graphServiceClient.identity.apiConnectors.post(requestBody);
}


```