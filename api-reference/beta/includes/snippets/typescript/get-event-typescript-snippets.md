---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
	}
,	queryParameters : {
		select: ["subject","body","bodyPreview","organizer","attendees","start","end","location","hideAttendees"],
	}
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").get(configuration);
}


```