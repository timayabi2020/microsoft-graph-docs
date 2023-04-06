---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BrowserSharedCookie = {
	hostOrDomain : "www.microsoft.com",
	sourceEnvironment : BrowserSharedCookieSourceEnvironment.MicrosoftEdge,
	displayName : "Microsoft Cookie",
	path : "/",
	hostOnly : true,
	comment : "Updating source environment.",
};

const result = async () => {
	await graphServiceClient.admin.edge.internetExplorerMode.siteListsById("browserSiteList-id").sharedCookiesById("browserSharedCookie-id").patch(requestBody);
}


```