---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AnswerPostRequestBody = {
	callbackUri : "callbackUri-value",
	mediaConfig : {
		"@odata.type" : "#microsoft.graph.appHostedMediaConfig",
		additionalData : {
			"blob" : "<Media Session Configuration Blob>",
		},
	},
	acceptedModalities : [
		modality : Modality.Audio,
	],
	callOptions : {
		"@odata.type" : "#microsoft.graph.incomingCallOptions",
		isContentSharingNotificationEnabled : true,
	},
	participantCapacity : 200,
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```