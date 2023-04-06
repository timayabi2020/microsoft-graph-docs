---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ValidatePropertiesPostRequestBody = {
	displayName : "Myprefix_test_mysuffix",
	mailNickname : "Myprefix_test_mysuffix",
	onBehalfOfUserId : "onBehalfOfUserId-value",
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").validateProperties.post(requestBody);
}


```