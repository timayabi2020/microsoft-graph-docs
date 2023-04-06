---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : FederationConfiguration = {
	additionalData : {
		"@odata.type" : "microsoft.graph.samlOrWsFedExternalDomainFederation",
		"issuerUri" : "https://contoso.com/issuerUri",
		"displayName" : "contoso display name",
		"metadataExchangeUri" : "https://contoso.com/metadataExchangeUri",
		"passiveSignInUri" : "https://contoso.com/signin",
		"preferredAuthenticationProtocol" : "wsFed",
		domains : [
			{
				"@odata.type" : "microsoft.graph.externalDomainName",
				id : "contoso.com",
			},
		],
		"signingCertificate" : "MIIDADCCAeigAwIBAgIQEX41y8r6",
	},
};

async () => {
	await graphServiceClient.directory.federationConfigurationsById("identityProviderBase-id").post(requestBody);
}


```