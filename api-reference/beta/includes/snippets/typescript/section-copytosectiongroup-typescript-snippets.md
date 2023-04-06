---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CopyToSectionGroupPostRequestBody = {
	id : "id-value",
	groupId : "groupId-value",
	renameAs : "renameAs-value",
};

const result = async () => {
	await graphServiceClient.me.onenote.sectionsById("onenoteSection-id").copyToSectionGroup.post(requestBody);
}


```