---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Calendar = {
	name : "Social events",
};

const result = async () => {
	await graphServiceClient.me.calendar.patch(requestBody);
}


```