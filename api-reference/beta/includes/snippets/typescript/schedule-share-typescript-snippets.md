---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SharePostRequestBody = {
	notifyTeam : true,
	startDateTime : new Date("2018-10-08T00:00:00.000Z"),
	endDateTime : new Date("2018-10-15T00:00:00.000Z"),
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.share.post(requestBody);
}


```