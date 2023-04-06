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
		content : "Does mid month work for you?",
	},
	start : {
		dateTime : "2019-03-15T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2019-03-15T14:00:00",
		timeZone : "Pacific Standard Time",
	},
	location : {
		displayName : "Harry's Bar",
	},
	attendees : [
		{
			emailAddress : {
				address : "adelev@contoso.onmicrosoft.com",
				name : "Adele Vance",
			},
			type : AttendeeType.Required,
		},
	],
	transactionId : "7E163156-7762-4BEB-A1C6-729EA81755A7",
};

const result = async () => {
	await graphServiceClient.me.calendarsById("calendar-id").events.post(requestBody);
}


```