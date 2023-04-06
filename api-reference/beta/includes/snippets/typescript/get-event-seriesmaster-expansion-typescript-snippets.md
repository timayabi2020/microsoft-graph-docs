---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["subject","start","end","occurrenceId","exceptionOccurrences","cancelledOccurrences"],
		expand: ["exceptionOccurrences"],
	}
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").get(configuration);
}


```