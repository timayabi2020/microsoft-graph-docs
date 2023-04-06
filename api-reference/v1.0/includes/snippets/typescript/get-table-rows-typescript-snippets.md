---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		top: 5,
		skip: 5,
	}
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.tablesById("workbookTable-id").rows.get(configuration);
}


```