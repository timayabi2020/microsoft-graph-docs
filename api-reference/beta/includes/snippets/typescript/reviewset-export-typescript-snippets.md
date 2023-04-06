---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExportPostRequestBody = {
	outputName : "2020-12-06 Contoso investigation export",
	description : "Export for the Contoso investigation",
	exportOptions : ExportOptions.OriginalFiles,fileInfo,tags,
	exportStructure : ExportFileStructure.Directory,
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").reviewSetsById("reviewSet-id").ediscoveryExport.post(requestBody);
}


```