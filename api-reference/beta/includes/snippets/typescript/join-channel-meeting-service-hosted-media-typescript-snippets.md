---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	"@odata.type" : "#microsoft.graph.call",
	callbackUri : "https://bot.contoso.com/callback",
	requestedModalities : [
		modality : Modality.Audio,
	],
	mediaConfig : {
		"@odata.type" : "#microsoft.graph.serviceHostedMediaConfig",
		additionalData : {
			preFetchMedia : [
				{
					uri : "https://cdn.contoso.com/beep.wav",
					resourceId : "f8971b04-b53e-418c-9222-c82ce681a582",
				},
				{
					uri : "https://cdn.contoso.com/cool.wav",
					resourceId : "86dc814b-c172-4428-9112-60f8ecae1edb",
				},
			],
		},
	},
	chatInfo : {
		"@odata.type" : "#microsoft.graph.chatInfo",
		threadId : "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
		messageId : "1533758867081",
	},
	meetingInfo : {
		"@odata.type" : "#microsoft.graph.organizerMeetingInfo",
		allowConversationWithoutHost : true,
		additionalData : {
			organizer : {
				"@odata.type" : "#microsoft.graph.identitySet",
				user : {
					"@odata.type" : "#microsoft.graph.identity",
					id : "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
					tenantId : "aa67bd4c-8475-432d-bd41-39f255720e0a",
					displayName : "Bob",
				},
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```