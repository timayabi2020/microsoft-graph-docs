---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ContactFolder = {
	parentFolderId : "parentFolderId-value",
	displayName : "displayName-value",
};

const result = async () => {
	await graphServiceClient.me.contactFoldersById("contactFolder-id").patch(requestBody);
}


```