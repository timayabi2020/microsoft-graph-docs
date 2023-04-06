---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "displayName eq 'AWS IAM Identity Center '",
	}
};

const result = async () => {
	await graphServiceClient.applicationTemplates.get(configuration);
}


```