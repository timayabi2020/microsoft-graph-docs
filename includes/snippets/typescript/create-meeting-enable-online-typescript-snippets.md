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
	subject : "Prep for customer meeting",
	body : {
		contentType : BodyType.HTML,
		content : "Does this time work for you?",
	},
	start : {
		dateTime : "2019-11-20T13:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2019-11-20T14:00:00",
		timeZone : "Pacific Standard Time",
	},
	location : {
		displayName : "Cordova conference room",
	},
	attendees : [
		{
			emailAddress : {
				address : "AdeleV@contoso.OnMicrosoft.com",
				name : "Adele Vance",
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