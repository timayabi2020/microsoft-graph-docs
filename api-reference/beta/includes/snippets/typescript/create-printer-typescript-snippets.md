---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CreatePostRequestBody = {
	displayName : "Test Printer",
	manufacturer : "Test Printer Manufacturer",
	model : "Test Printer Model",
	physicalDeviceId : null,
	hasPhysicalDevice : false,
	certificateSigningRequest : {
		content : "{content}",
		transportKey : "{sampleTransportKey}",
	},
	connectorId : null,
};

const result = async () => {
	await graphServiceClient.print.printers.create.post(requestBody);
}


```