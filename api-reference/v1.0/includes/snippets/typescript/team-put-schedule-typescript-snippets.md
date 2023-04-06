---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Schedule = {
	enabled : true,
	timeZone : "America/Chicago",
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.put(requestBody);
}


```