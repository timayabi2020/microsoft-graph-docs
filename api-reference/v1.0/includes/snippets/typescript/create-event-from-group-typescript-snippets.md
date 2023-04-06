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
		content : "Does late morning work for you?",
	},
	start : {
		dateTime : "2019-06-16T12:00:00",
		timeZone : "Pacific Standard Time",
	},
	end : {
		dateTime : "2019-06-16T14:00:00",
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
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").events.post(requestBody);
}


```