---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BrowserSite = {
	webUrl : "www.microsoft.com",
	targetEnvironment : BrowserSiteTargetEnvironment.MicrosoftEdge,
	mergeType : BrowserSiteMergeType.Default,
	compatibilityMode : BrowserSiteCompatibilityMode.Default,
	allowRedirect : false,
	comment : "Updating to Edge.",
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteListsById("browserSiteList-id").sitesById("browserSite-id").patch(requestBody);
}


```