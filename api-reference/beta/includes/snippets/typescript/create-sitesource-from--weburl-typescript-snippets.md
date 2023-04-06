---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SiteSource = {
	site : {
		webUrl : "https://m365x809305.sharepoint.com/sites/Retail",
	},
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").legalHoldsById("ediscoveryHoldPolicy-id").siteSources.post(requestBody);
}


```