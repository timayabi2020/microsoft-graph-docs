---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetNotebookFromWebUrlPostRequestBody = {
	webUrl : "webUrl value",
};

const result = async () => {
	await graphServiceClient.me.onenote.notebooks.getNotebookFromWebUrl.post(requestBody);
}


```