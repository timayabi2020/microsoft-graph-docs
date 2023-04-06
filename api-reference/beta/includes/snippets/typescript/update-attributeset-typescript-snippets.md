---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AttributeSet = {
	description : "Attributes for engineering team",
	maxAttributesPerSet : 20,
};

const result = async () => {
	await graphServiceClient.directory.attributeSetsById("attributeSet-id").patch(requestBody);
}


```