---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetByIdsPostRequestBody = {
	ids : [
		"84b80893-8749-40a3-97b7-68513b600544",
		"5d6059b6-368d-45f8-91e1-8e07d485f1d0",
		"0b944de3-e0fc-4774-a49a-b135213725ef",
		"b75a5ab2-fe55-4463-bd31-d21ad555c6e0",
	],
	types : [
		"user",
		"group",
		"device",
	],
};

const result = async () => {
	await graphServiceClient.directoryObjects.getByIds.post(requestBody);
}


```