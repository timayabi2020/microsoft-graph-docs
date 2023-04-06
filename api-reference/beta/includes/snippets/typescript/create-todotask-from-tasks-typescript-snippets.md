---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TodoTask = {
	title : "A new task",
	categories : [
		"Important",
	],
	linkedResources : [
		{
			webUrl : "http://microsoft.com",
			applicationName : "Microsoft",
			displayName : "Microsoft",
		},
	],
};

const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasks.post(requestBody);
}


```