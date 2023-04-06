---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BrowserSite = {
	"@odata.type" : "#microsoft.graph.browserSite",
	webUrl : "www.microsoft.com",
	targetEnvironment : BrowserSiteTargetEnvironment.InternetExplorer11,
	comment : "A site that opens in InternetExplorer11",
	mergeType : BrowserSiteMergeType.Default,
	compatibilityMode : BrowserSiteCompatibilityMode.Default,
	allowRedirect : true,
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteListsById("browserSiteList-id").sites.post(requestBody);
}


```