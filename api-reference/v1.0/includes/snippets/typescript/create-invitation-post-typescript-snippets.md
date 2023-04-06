---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Invitation = {
	invitedUserEmailAddress : "admin@fabrikam.com",
	inviteRedirectUrl : "https://myapp.contoso.com",
};

const result = async () => {
	await graphServiceClient.invitations.post(requestBody);
}


```