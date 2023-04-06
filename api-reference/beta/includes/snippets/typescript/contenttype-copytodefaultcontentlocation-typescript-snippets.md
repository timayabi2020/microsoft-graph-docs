---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CopyToDefaultContentLocationPostRequestBody = {
	sourceFile : {
		sharepointIds : {
			listId : "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
			listItemId : "2",
		},
	},
	destinationFileName : "newname.txt",
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").contentTypesById("contentType-id").copyToDefaultContentLocation.post(requestBody);
}


```