---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Accept": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
	}
,	queryParameters : {
		format: "text/vtt",
	}
};

const result = async () => {
	await graphServiceClient.usersById("user-id").onlineMeetingsById("onlineMeeting-id").transcriptsById("callTranscript-id").content.get(configuration);
}


```