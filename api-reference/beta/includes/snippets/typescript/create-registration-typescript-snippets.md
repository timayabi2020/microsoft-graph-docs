---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RegistrationPostRequestBody = {
	additionalData : {
		"@odata.type" : "#microsoft.graph.meetingRegistration",
		"subject" : "Microsoft Ignite",
		"description" : "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
		"startDateTime" : "2021-11-02T08:00:00-08:00",
		"endDateTime" : "2021-11-04T04:00:00-08:00",
		"allowedRegistrant" : "everyone",
		speakers : [
			{
				displayName : "Henry Ross",
				bio : "Chairman and Chief Executive Officer",
			},
			{
				displayName : "Hailey Clark",
				bio : "EVP",
			},
		],
		customQuestions : [
			{
				displayName : "Are you a developer?",
				answerInputType : "radioButton",
				answerOptions : [
					"Yes",
					"No",
				],
				isRequired : true,
			},
			{
				displayName : "Where did you hear about us?",
				answerInputType : "text",
				isRequired : false,
			},
		],
	},
};

async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.post(requestBody);
}


```