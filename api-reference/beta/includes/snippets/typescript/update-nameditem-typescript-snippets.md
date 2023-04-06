---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkbookNamedItem = {
	type : "type-value",
	scope : "scope-value",
	comment : "comment-value",
	value : {
	},
	visible : true,
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.namesById("workbookNamedItem-id").patch(requestBody);
}


```