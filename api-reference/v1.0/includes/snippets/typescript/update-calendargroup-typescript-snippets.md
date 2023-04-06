---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CalendarGroup = {
	name : "name-value",
};

const result = async () => {
	await graphServiceClient.me.calendarGroupsById("calendarGroup-id").patch(requestBody);
}


```