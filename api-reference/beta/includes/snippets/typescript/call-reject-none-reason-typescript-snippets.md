---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RejectPostRequestBody = {
	reason : RejectReason.None,
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").reject.post(requestBody);
}


```