---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Invitation = {
	invitedUserDisplayName : "John Doe (Tailspin Toys)",
	invitedUserEmailAddress : "john@tailspintoys.com",
	sendInvitationMessage : false,
	inviteRedirectUrl : "https://myapps.microsoft.com",
};

const result = async () => {
	await graphServiceClient.invitations.post(requestBody);
}


```