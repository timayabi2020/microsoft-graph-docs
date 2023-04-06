---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MeetingRegistration = {
	subject : "Microsoft Ignite: Day 1",
	startDateTime : new Date("2021-11-02T08:00:00-08:00"),
	endDateTime : new Date("2021-11-02T15:45:00-08:00"),
	speakers : [
		{
			displayName : "Henry Ross",
			bio : "Chairman and Chief Executive Officer",
		},
		{
			displayName : "Fred Ryan",
			bio : "CVP",
		},
	],
};

const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.patch(requestBody);
}


```