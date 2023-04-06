---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Contact = {
	parentFolderId : "parentFolderId-value",
	birthday : new Date("datetime-value"),
	fileAs : "fileAs-value",
	displayName : "displayName-value",
	givenName : "givenName-value",
	initials : "initials-value",
};

const result = async () => {
	await graphServiceClient.me.contactFoldersById("contactFolder-id").contacts.post(requestBody);
}


```