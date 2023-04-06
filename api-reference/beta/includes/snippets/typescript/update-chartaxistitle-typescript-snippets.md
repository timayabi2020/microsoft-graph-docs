---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkbookChartAxisTitle = {
	text : "text-value",
	visible : true,
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").chartsById("workbookChart-id").axes.valueAxis.title.patch(requestBody);
}


```