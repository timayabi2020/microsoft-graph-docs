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
};
const requestBody : OutlookTask = {
	subject : "Shop for children's weekend",
	startDateTime : {
		dateTime : "2016-05-03T09:00:00",
		timeZone : "Eastern Standard Time",
	},
	dueDateTime : {
		dateTime : "2016-05-05T16:00:00",
		timeZone : "Eastern Standard Time",
	},
};

const result = async () => {
	await graphServiceClient.me.outlook.tasks.post(requestBody, configuration);
}


```