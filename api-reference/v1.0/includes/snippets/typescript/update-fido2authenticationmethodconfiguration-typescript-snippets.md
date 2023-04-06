---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationMethodConfiguration = {
	"@odata.type" : "#microsoft.graph.fido2AuthenticationMethodConfiguration",
	state : AuthenticationMethodState.Enabled,
	additionalData : {
		"isAttestationEnforced" : "true",
	},
};

const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsById("authenticationMethodConfiguration-id").patch(requestBody);
}


```