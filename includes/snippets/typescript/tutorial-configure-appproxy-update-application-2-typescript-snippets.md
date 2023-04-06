---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	onPremisesPublishing : {
		externalAuthenticationType : ExternalAuthenticationType.AadPreAuthentication,
		internalUrl : "https://contosoiwaapp.com",
		externalUrl : "https://contosoiwaapp-contoso.msappproxy.net",
		isHttpOnlyCookieEnabled : true,
		isOnPremPublishingEnabled : true,
		isPersistentCookieEnabled : true,
		isSecureCookieEnabled : true,
		isStateSessionEnabled : true,
		isTranslateHostHeaderEnabled : true,
		isTranslateLinksInBodyEnabled : true,
	},
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```