---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	subject : "Annual review",
	body : {
		contentType : BodyType.HTML,
		content : "You should be proud!",
	},
	toRecipients : [
		{
			emailAddress : {
				address : "rufus@contoso.com",
			},
		},
	],
	extensions : [
		{
			"@odata.type" : "microsoft.graph.openTypeExtension",
			additionalData : {
				"extensionName" : "Com.Contoso.Referral",
				"companyName" : "Wingtip Toys",
				"expirationDate" : "2015-12-30T11:00:00.000Z",
				dealValue : 10000,
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```