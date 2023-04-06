---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Printer = {
	location : {
		latitude : 1.1,
		longitude : 2.2,
		altitudeInMeters : 3,
	},
	additionalData : {
		"name" : "PrinterName",
	},
};

const result = async () => {
	await graphServiceClient.print.printersById("printer-id").patch(requestBody);
}


```