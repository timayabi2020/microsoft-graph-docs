---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OutlookTask = {
	subject : "Shop for dinner",
	startDateTime : {
		dateTime : "2016-04-23T18:00:00",
		timeZone : "Pacific Standard Time",
	},
	dueDateTime : {
		dateTime : "2016-04-25T13:00:00",
		timeZone : "Pacific Standard Time",
	},
};

const result = async () => {
	await graphServiceClient.me.outlook.taskFoldersById("outlookTaskFolder-id").tasks.post(requestBody);
}


```