---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TodoTask = {
	dueDateTime : {
		dateTime : "2020-07-25T16:00:00",
		timeZone : "Eastern Standard Time",
	},
};

const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasksById("todoTask-id").patch(requestBody);
}


```