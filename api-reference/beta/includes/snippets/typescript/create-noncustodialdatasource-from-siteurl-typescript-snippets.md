---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NoncustodialDataSource = {
	applyHoldToSource : false,
	dataSource : {
		"@odata.type" : "microsoft.graph.ediscovery.siteSource",
		additionalData : {
			site : {
				webUrl : "https://contoso.sharepoint.com/sites/SecretSite",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").noncustodialDataSources.post(requestBody);
}


```