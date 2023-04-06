---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AssociateWithHubSitesPostRequestBody = {
	hubSiteUrls : [
		"https://graph.microsoft.com/v1.0/sites/{site-id}",
	],
	propagateToExistingLists : false,
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").contentTypesById("contentType-id").associateWithHubSites.post(requestBody);
}


```