---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Event = {
	subject : "Let's go for lunch",
	body : {
		contentType : BodyType.HTML,
		content : "Does noon time work for you?",
	},
	start : {
		dateTime : "2017-09-04T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2017-09-04T14:00:00",
		timeZone : "Pacific Standard Time",
	},
	recurrence : {
		pattern : {
			type : RecurrencePatternType.Weekly,
			interval : 1,
			daysOfWeek : [
				dayOfWeek : DayOfWeek.Monday,
			],
		},
		range : {
			type : RecurrenceRangeType.EndDate,
			startDate : "2017-09-04",
			endDate : "2017-12-31",
		},
	},
	location : {
		displayName : "Harry's Bar",
	},
	attendees : [
		{
			emailAddress : {
				address : "AdeleV@contoso.onmicrosoft.com",
				name : "Adele Vance",
			},
			type : AttendeeType.Required,
		},
	],
	allowNewTimeProposals : true,
};

const result = async () => {
	await graphServiceClient.me.events.post(requestBody);
}


```