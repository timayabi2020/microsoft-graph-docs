---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedGroupSource = {
	group : {
		mail : "SOCTeam@M365x809305.onmicrosoft.com",
	},
	includedSources : SourceType.Mailbox, site,
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").custodiansById("ediscoveryCustodian-id").unifiedGroupSources.post(requestBody);
}


```