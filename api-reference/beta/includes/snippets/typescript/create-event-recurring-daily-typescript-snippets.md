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
const requestBody : Event = {
	subject : "Let's go for lunch",
	body : {
		contentType : BodyType.HTML,
		content : "Does noon work for you?",
	},
	start : {
		dateTime : "2020-02-25T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2020-02-25T14:00:00",
		timeZone : "Pacific Standard Time",
	},
	location : {
		displayName : "Harry's Bar",
	},
	attendees : [
		{
			emailAddress : {
				address : "AlexW@contoso.OnMicrosoft.com",
				name : "Alex Wilbur",
			},
			type : AttendeeType.Required,
		},
	],
	recurrence : {
		pattern : {
			type : RecurrencePatternType.Daily,
			interval : 1,
		},
		range : {
			type : RecurrenceRangeType.Numbered,
			startDate : "2020-02-25",
			numberOfOccurrences : 2,
		},
	},
};

const result = async () => {
	await graphServiceClient.me.events.post(requestBody, configuration);
}


```