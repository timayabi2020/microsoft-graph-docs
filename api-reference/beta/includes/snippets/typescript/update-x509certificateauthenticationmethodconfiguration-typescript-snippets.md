---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationMethodConfiguration = {
	"@odata.type" : "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
	id : "X509Certificate",
	state : AuthenticationMethodState.Enabled,
	additionalData : {
		certificateUserBindings : [
			{
				x509CertificateField : "PrincipalName",
				userProperty : "onPremisesUserPrincipalName",
				priority : 1,
			},
		],
		authenticationModeConfiguration : {
			x509CertificateAuthenticationDefaultMode : "x509CertificateMultiFactor",
			rules : [
				{
					x509CertificateRuleType : "issuerSubject",
					identifier : "CN=ContosoCA,DC=Contoso,DC=org ",
					x509CertificateAuthenticationMode : "x509CertificateMultiFactor",
				},
				{
					x509CertificateRuleType : "policyOID",
					identifier : "1.2.3.4",
					x509CertificateAuthenticationMode : "x509CertificateMultiFactor",
				},
			],
		},
		includeTargets : [
			{
				targetType : "group",
				id : "all_users",
				isRegistrationRequired : false,
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsById("authenticationMethodConfiguration-id").patch(requestBody);
}


```