---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InternalDomainFederation = {
	"@odata.type" : "#microsoft.graph.internalDomainFederation",
	displayName : "Contoso",
	issuerUri : "http://contoso.com/adfs/services/trust",
	metadataExchangeUri : "https://sts.contoso.com/adfs/services/trust/mex",
	signingCertificate : "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
	passiveSignInUri : "https://sts.contoso.com/adfs/ls",
	preferredAuthenticationProtocol : AuthenticationProtocol.WsFed,
	activeSignInUri : "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
	signOutUri : "https://sts.contoso.com/adfs/ls",
	promptLoginBehavior : PromptLoginBehavior.NativeSupport,
	isSignedAuthenticationRequestRequired : true,
	nextSigningCertificate : "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
	federatedIdpMfaBehavior : FederatedIdpMfaBehavior.RejectMfaByFederatedIdp,
};

const result = async () => {
	await graphServiceClient.domainsById("domain-id").federationConfiguration.post(requestBody);
}


```