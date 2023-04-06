---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Bookmark = {
	displayName : "Contoso Install Site",
	webUrl : "http://www.contoso.com/",
	description : "Try or buy Contoso for Home or Business and view product information",
	keywords : {
		keywords : [
			"Contoso",
			"install",
		],
		reservedKeywords : [
			"Contoso",
		],
		matchSimilarKeywords : true,
	},
	state : AnswerState.Published,
};

const result = async () => {
	await graphServiceClient.search.bookmarks.post(requestBody);
}


```