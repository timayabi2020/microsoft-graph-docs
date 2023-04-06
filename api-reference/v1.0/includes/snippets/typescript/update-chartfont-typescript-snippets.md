---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkbookChartFont = {
	bold : true,
	color : "color-value",
	italic : true,
	name : "name-value",
	size : 99,
	underline : "underline-value",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").chartsById("workbookChart-id").axes.valueAxis.format.font.patch(requestBody);
}


```