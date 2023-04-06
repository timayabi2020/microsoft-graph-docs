---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ApplyPostRequestBody = {
	fields : [
		{
			key : 99,
			sortOn : "sortOn-value",
			ascending : true,
			color : "color-value",
			dataOption : "dataOption-value",
			icon : {
				set : "set-value",
				index : 99,
			},
		},
	],
	matchCase : true,
	method : "method-value",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.tablesById("workbookTable-id").sort.apply.post(requestBody);
}


```