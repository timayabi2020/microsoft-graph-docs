---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExportPostRequestBody = {
	outputName : "Export via API",
	description : "Export for the Contoso investigation",
	exportOptions : ExportOptions.OriginalFiles,fileInfo,tags,
	exportStructure : ExportFileStructure.Directory,
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCasesById("ediscoveryCase-id").reviewSetsById("ediscoveryReviewSet-id").securityExport.post(requestBody);
}


```