---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OnlineMeeting = {
	startDateTime : new Date("2019-07-12T14:30:34.2444915-07:00"),
	endDateTime : new Date("2019-07-12T15:00:34.2464912-07:00"),
	subject : "User Token Meeting",
};

const result = async () => {
	await graphServiceClient.me.onlineMeetings.post(requestBody);
}


```