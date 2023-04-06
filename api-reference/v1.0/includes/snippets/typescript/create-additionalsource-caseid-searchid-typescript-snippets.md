---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DataSource = {
	"@odata.type" : "microsoft.graph.security.siteSource",
	additionalData : {
		site : {
			webUrl : "https://contoso.sharepoint.com/sites/SecretSite",
		},
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").searchesById("ediscoverySearch-id").additionalSources.post(requestBody);
}


```