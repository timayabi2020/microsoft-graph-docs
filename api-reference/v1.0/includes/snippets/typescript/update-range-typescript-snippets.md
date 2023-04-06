---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Range(address='{address}')PatchRequestBody = {
	additionalData : {
		values : [
			 : [
				"Hello",
				"100",
			],
			 : [
				"1/1/2016",
				 : null,
			],
		],
		formulas : [
			 : [
				 : null,
				 : null,
			],
			 : [
				 : null,
				"=B1*2",
			],
		],
		numberFormat : [
			 : [
				 : null,
				 : null,
			],
			 : [
				"m-ddd",
				 : null,
			],
		],
	},
};

async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.worksheetsById("workbookWorksheet-id").range(address='{address}').patch(requestBody);
}


```