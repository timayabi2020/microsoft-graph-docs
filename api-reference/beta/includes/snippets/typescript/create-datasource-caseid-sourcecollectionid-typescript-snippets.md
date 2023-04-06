---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DataSource = {
	"@odata.type" : "microsoft.graph.ediscovery.userSource",
	additionalData : {
		"email" : "badguy@contoso.com",
	},
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").sourceCollectionsById("sourceCollection-id").additionalSources.post(requestBody);
}


```