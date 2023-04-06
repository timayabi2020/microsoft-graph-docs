---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddPostRequestBody = {
	index : 5,
	values : [
		Json : [
			 : 1,
			 : 2,
			 : 3,
		],
		Json : [
			 : 4,
			 : 5,
			 : 6,
		],
	],
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.tablesById("workbookTable-id").rows.add.post(requestBody);
}


```