---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BrowserSharedCookie = {
	"@odata.type" : "#microsoft.graph.browserSharedCookie",
	hostOrDomain : "www.microsoft.com",
	sourceEnvironment : BrowserSharedCookieSourceEnvironment.InternetExplorer11,
	displayName : "Microsoft Cookie",
	hostOnly : true,
	comment : "A cookie for microsoft.com",
	path : "/",
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteListsById("browserSiteList-id").sharedCookies.post(requestBody);
}


```