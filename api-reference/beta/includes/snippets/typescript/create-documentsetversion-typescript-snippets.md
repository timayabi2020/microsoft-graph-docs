---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DocumentSetVersion = {
	comment : "v1",
	shouldCaptureMinorVersion : false,
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").itemsById("listItem-id").documentSetVersions.post(requestBody);
}


```