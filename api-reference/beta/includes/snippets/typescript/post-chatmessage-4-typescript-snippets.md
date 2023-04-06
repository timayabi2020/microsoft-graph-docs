---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	body : {
		contentType : BodyType.Html,
		content : "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>",
	},
	attachments : [
		{
			id : "153fa47d-18c9-4179-be08-9879815a9f90",
			contentType : "reference",
			contentUrl : "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
			name : "Budget.docx",
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```