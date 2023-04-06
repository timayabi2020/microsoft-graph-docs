---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		startDateTime: "2019-04-08T09:00:00.0000000",
		endDateTime: "2019-04-30T09:00:00.0000000",
		select: ["subject","bodyPreview","seriesMasterId","type","recurrence","start","end"],
	}
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").instances.get(configuration);
}


```