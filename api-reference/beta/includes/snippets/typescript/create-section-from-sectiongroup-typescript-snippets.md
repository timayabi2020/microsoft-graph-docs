---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OnenoteSection = {
	displayName : "Section name",
};

const result = async () => {
	await graphServiceClient.me.onenote.sectionGroupsById("sectionGroup-id").sections.post(requestBody);
}


```