---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UpdateRecordingStatusPostRequestBody = {
	clientContext : "clientContext-value",
	status : RecordingStatus.NotRecording | recording | failed,
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").updateRecordingStatus.post(requestBody);
}


```