---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CopyNotebookPostRequestBody = {
	groupId : "groupId-value",
	renameAs : "renameAs-value",
};

const result = async () => {
	await graphServiceClient.me.onenote.notebooksById("notebook-id").copyNotebook.post(requestBody);
}


```