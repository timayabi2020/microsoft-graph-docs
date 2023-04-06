---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkbookTable = {
	name : "name-value",
	showHeaders : true,
	showTotals : true,
	style : "style-value",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.tablesById("workbookTable-id").patch(requestBody);
}


```