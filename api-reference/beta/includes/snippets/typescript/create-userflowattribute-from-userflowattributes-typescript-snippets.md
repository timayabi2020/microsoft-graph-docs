---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityUserFlowAttribute = {
	displayName : "Hobby",
	description : "Your hobby",
	dataType : IdentityUserFlowAttributeDataType.String,
};

const result = async () => {
	await graphServiceClient.identity.userFlowAttributes.post(requestBody);
}


```