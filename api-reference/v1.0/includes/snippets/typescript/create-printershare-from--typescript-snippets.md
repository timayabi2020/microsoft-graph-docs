---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrinterShare = {
	displayName : "ShareName",
	allowAllUsers : false,
	additionalData : {
		"printer@odata.bind" : "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
	},
};

const result = async () => {
	await graphServiceClient.print.shares.post(requestBody);
}


```