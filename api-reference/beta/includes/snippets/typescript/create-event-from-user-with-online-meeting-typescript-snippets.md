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
		dateTime : "2017-04-15T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2017-04-15T14:00:00",
		timeZone : "Pacific Standard Time",
	},
	location : {
		displayName : "Harry's Bar",
	},
	attendees : [
		{
			emailAddress : {
				address : "samanthab@contoso.onmicrosoft.com",
				name : "Samantha Booth",
			},
			type : AttendeeType.Required,
		},
	],
	allowNewTimeProposals : true,
	isOnlineMeeting : true,
	onlineMeetingProvider : OnlineMeetingProviderType.TeamsForBusiness,
};

const result = async () => {
	await graphServiceClient.me.events.post(requestBody, configuration);
}


```