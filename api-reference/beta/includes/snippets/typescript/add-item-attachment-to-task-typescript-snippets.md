---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Attachment = {
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
				dateTime : "2020-01-12T18:00:00",
				timeZone : "Pacific Standard Time",
			},
			end : {
				dateTime : "2020-01-12T19:00:00",
				timeZone : "Pacific Standard Time",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.me.outlook.tasksById("outlookTask-id").attachments.post(requestBody);
}


```