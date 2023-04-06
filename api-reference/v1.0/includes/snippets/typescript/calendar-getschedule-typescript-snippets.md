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
const requestBody : GetSchedulePostRequestBody = {
	schedules : [
		"adelev@contoso.onmicrosoft.com",
		"meganb@contoso.onmicrosoft.com",
	],
	startTime : {
		dateTime : "2019-03-15T09:00:00",
		timeZone : "Pacific Standard Time",
	},
	endTime : {
		dateTime : "2019-03-15T18:00:00",
		timeZone : "Pacific Standard Time",
	},
	availabilityViewInterval : 60,
};

const result = async () => {
	await graphServiceClient.me.calendar.getSchedule.post(requestBody, configuration);
}


```