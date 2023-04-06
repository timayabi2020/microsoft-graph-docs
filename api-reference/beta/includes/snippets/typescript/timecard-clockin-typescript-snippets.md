---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ClockInPostRequestBody = {
	notes : {
		contentType : BodyType.Text,
		content : "clock in notes",
	},
	additionalData : {
		atAprovedLocation : true,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCards.clockIn.post(requestBody);
}


```