---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TranslateExchangeIdsPostRequestBody = {
	inputIds : [
		"{rest-formatted-id-1}",
		"{rest-formatted-id-2}",
	],
	sourceIdType : ExchangeIdFormat.RestId,
	targetIdType : ExchangeIdFormat.RestImmutableEntryId,
};

const result = async () => {
	await graphServiceClient.me.translateExchangeIds.post(requestBody);
}


```