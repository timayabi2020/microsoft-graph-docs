---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ColumnDefinition = {
	additionalData : {
		"sourceColumn@odata.bind" : "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
	},
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").contentTypesById("contentType-id").columns.post(requestBody);
}


```