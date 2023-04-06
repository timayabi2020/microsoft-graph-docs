---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReplyPostRequestBody = {
	post : {
		body : {
			contentType : BodyType.Text,
			content : "I attached an event.",
		},
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.itemAttachment",
				name : "Holiday event",
				additionalData : {
					item : {
						"@odata.type" : "microsoft.graph.event",
						subject : "Discuss gifts for children",
						body : {
							contentType : "HTML",
							content : "Let's look for funding!",
						},
						start : {
							dateTime : "2019-12-02T18:00:00",
							timeZone : "Pacific Standard Time",
						},
						end : {
							dateTime : "2019-12-02T19:00:00",
							timeZone : "Pacific Standard Time",
						},
					},
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```