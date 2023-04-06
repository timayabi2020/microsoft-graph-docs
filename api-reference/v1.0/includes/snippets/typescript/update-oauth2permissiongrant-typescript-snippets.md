---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OAuth2PermissionGrant = {
	scope : "User.ReadBasic.All Group.ReadWrite.All",
};

const result = async () => {
	await graphServiceClient.oauth2PermissionGrantsById("oAuth2PermissionGrant-id").patch(requestBody);
}


```