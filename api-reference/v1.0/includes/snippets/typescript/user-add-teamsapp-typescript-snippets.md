---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UserScopeTeamsAppInstallation = {
	additionalData : {
		"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").teamwork.installedApps.post(requestBody);
}


```