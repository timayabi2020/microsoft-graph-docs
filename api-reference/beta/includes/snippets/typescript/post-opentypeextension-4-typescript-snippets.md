---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReplyPostRequestBody = {
	post : {
		body : {
			contentType : BodyType.Html,
			content : "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>",
		},
		extensions : [
			{
				"@odata.type" : "microsoft.graph.openTypeExtension",
				additionalData : {
					"extensionName" : "Com.Contoso.HR",
					"companyName" : "Contoso",
					"expirationDate" : "2015-07-03T13:04:00.000Z",
					topPicks : [
						"Employees only",
						"Add spouse or guest",
						"Add family",
					],
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").postsById("post-id").reply.post(requestBody);
}


```