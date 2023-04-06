---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "outlook.timezone=\"Eastern Standard Time\"",
	}
};
const requestBody : OutlookTask = {
	dueDateTime : {
		dateTime : "2016-05-06T16:00:00",
		timeZone : "Eastern Standard Time",
	},
};

const result = async () => {
	await graphServiceClient.me.outlook.tasksById("outlookTask-id").patch(requestBody, configuration);
}


```