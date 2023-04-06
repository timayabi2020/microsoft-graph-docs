---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProtectPostRequestBody = {
	options : {
		allowFormatCells : true,
		allowFormatColumns : true,
		allowFormatRows : true,
		allowInsertColumns : true,
		allowInsertRows : true,
		allowInsertHyperlinks : true,
		allowDeleteColumns : true,
		allowDeleteRows : true,
		allowSort : true,
		allowAutoFilter : true,
		allowPivotTables : true,
	},
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").protection.protect.post(requestBody);
}


```