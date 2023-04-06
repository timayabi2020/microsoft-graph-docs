---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TeamsTab = {
	displayName : "My Contoso Tab",
	configuration : {
		entityId : "2DCA2E6C7A10415CAF6B8AB6661B3154",
		contentUrl : "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
		websiteUrl : "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
		removeUrl : "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab",
	},
	additionalData : {
		"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
	},
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").tabs.post(requestBody);
}


```