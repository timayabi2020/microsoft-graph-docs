---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SitePage = {
	"@odata.type" : "#microsoft.graph.sitePage",
	title : "sample",
	showComments : true,
	showRecommendedPages : false,
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").pagesById("sitePage-id").patch(requestBody);
}


```