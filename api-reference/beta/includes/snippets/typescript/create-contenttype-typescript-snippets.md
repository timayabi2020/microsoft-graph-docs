---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ContentType = {
	name : "docSet",
	description : "custom docset",
	base : {
		name : "Document Set",
		id : "0x0120D520",
	},
	group : "Document Set Content Types",
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").contentTypes.post(requestBody);
}


```