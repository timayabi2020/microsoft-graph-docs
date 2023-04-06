---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Serie = {
	additionalData : {
		index : 2,
	},
};

async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").chartsById("workbookChart-id").seriesById("workbookChartSeries-id").post(requestBody);
}


```