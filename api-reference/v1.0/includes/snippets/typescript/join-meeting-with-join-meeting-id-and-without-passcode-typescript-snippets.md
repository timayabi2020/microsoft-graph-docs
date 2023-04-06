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
	meetingInfo : {
		"@odata.type" : "#microsoft.graph.joinMeetingIdMeetingInfo",
		additionalData : {
			"joinMeetingId" : "1234567",
			passcode : null,
		},
	},
	tenantId : "86dc81db-c112-4228-9222-63f3esaa1edb",
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```