---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : B2xIdentityUserFlow = {
	id : "UserFlowWithAPIConnector",
	userFlowType : UserFlowType.SignUpOrSignIn,
	userFlowTypeVersion : 1,
	apiConnectorConfiguration : {
		postFederationSignup : {
			additionalData : {
				"@odata.id" : "{apiConnectorId}",
			},
		},
		postAttributeCollection : {
			additionalData : {
				"@odata.id" : "{apiConnectorId}",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.identity.b2xUserFlows.post(requestBody);
}


```