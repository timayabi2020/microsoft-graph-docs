---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		forcedelete: true,
	}
};

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").tagsById("tag-id").delete(configuration);
}


```