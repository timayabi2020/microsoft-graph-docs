---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddFormulaLocalPostRequestBody = {
	name : "test7",
	formula : "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
	comment : "Comment for the named item",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").workbook.names.addFormulaLocal.post(requestBody);
}


```