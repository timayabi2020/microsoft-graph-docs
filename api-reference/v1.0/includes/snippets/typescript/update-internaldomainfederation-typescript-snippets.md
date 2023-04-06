---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : InternalDomainFederation = {
	displayName : "Contoso name change",
	federatedIdpMfaBehavior : FederatedIdpMfaBehavior.AcceptIfMfaDoneByFederatedIdp,
};

const result = async () => {
	await graphServiceClient.domainsById("domain-id").federationConfigurationById("internalDomainFederation-id").patch(requestBody);
}


```