---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MailFolder = {
	"@odata.type" : "microsoft.graph.mailSearchFolder",
	displayName : "Weekly digests",
	additionalData : {
		includeNestedFolders : true,
		sourceFolderIds : [
			"AQMkADYAAAIBDAAAAA==",
		],
		"filterQuery" : "contains(subject, 'weekly digest')",
	},
};

const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").childFolders.post(requestBody);
}


```