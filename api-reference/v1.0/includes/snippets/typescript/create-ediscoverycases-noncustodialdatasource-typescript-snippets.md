---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NoncustodialSource = {
	additionalData : {
		"@odata.id" : "https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339",
	},
};

async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").searchesById("ediscoverySearch-id").noncustodialSourcesById("ediscoveryNoncustodialDataSource-id").post(requestBody);
}


```