---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TentativelyAcceptPostRequestBody = {
	comment : "I will probably be able to make it.",
	sendResponse : true,
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").tentativelyAccept.post(requestBody);
}


```