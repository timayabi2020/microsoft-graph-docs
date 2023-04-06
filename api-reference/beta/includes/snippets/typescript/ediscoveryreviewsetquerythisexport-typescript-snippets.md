---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExportPostRequestBody = {
	outputName : "Export reviewset query via API",
	description : "Export for the Contoso investigation 2",
	exportOptions : ExportOptions.OriginalFiles,fileInfo,tags,
	exportStructure : ExportFileStructure.Directory,
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").reviewSetsById("ediscoveryReviewSet-id").queriesById("ediscoveryReviewSetQuery-id").securityExport.post(requestBody);
}


```