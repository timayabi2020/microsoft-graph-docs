---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Call = {
	"@odata.type" : "#microsoft.graph.call",
	direction : CallDirection.Outgoing,
	callbackUri : "https://bot.contoso.com/callback",
	requestedModalities : [
		modality : Modality.Audio,
	],
	mediaConfig : {
		"@odata.type" : "#microsoft.graph.appHostedMediaConfig",
		additionalData : {
			"blob" : "<Media Session Configuration>",
		},
	},
	chatInfo : {
		"@odata.type" : "#microsoft.graph.chatInfo",
		threadId : "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
		messageId : "0",
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
	tenantId : "aa67bd4c-8475-432d-bd41-39f255720e0a",
};

const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```