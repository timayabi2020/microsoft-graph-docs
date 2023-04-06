---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : StartBreakPostRequestBody = {
	notes : {
		contentType : BodyType.Text,
		content : "start break smaple notes",
	},
	additionalData : {
		atAprovedLocation : true,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCardsById("timeCard-id").startBreak.post(requestBody);
}


```