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
	subject : "Plan summer company picnic",
	body : {
		contentType : BodyType.HTML,
		content : "Let's kick-start this event planning!",
	},
	start : {
		dateTime : "2017-08-30T11:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2017-08-30T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	attendees : [
		{
			emailAddress : {
				address : "DanaS@contoso.onmicrosoft.com",
				name : "Dana Swope",
			},
			type : AttendeeType.Required,
		},
		{
			emailAddress : {
				address : "AlexW@contoso.onmicrosoft.com",
				name : "Alex Wilber",
			},
			type : AttendeeType.Required,
		},
	],
	location : {
		displayName : "Conf Room 3; Fourth Coffee; Home Office",
		locationType : LocationType.Default,
	},
	locations : [
		{
			displayName : "Conf Room 3",
		},
		{
			displayName : "Fourth Coffee",
			address : {
				street : "4567 Main St",
				city : "Redmond",
				state : "WA",
				countryOrRegion : "US",
				postalCode : "32008",
			},
			coordinates : {
				latitude : 47.672,
				longitude : -102.103,
			},
		},
		{
			displayName : "Home Office",
		},
	],
	allowNewTimeProposals : true,
};

const result = async () => {
	await graphServiceClient.me.events.post(requestBody, configuration);
}


```