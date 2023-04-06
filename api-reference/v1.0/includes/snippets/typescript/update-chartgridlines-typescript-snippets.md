---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkbookChartGridlines = {
	visible : true,
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").chartsById("workbookChart-id").axes.valueAxis.minorGridlines.patch(requestBody);
}


```