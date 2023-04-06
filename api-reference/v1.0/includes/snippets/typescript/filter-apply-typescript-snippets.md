---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ApplyPostRequestBody = {
	criteria : {
		criterion1 : "criterion1-value",
		criterion2 : "criterion2-value",
		color : "color-value",
		operator : {
		},
		icon : {
			set : "set-value",
			index : 99,
		},
		dynamicCriteria : "dynamicCriteria-value",
		values : {
		},
		filterOn : "filterOn-value",
	},
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.tablesById("workbookTable-id").columnsById("workbookTableColumn-id").filter.apply.post(requestBody);
}


```