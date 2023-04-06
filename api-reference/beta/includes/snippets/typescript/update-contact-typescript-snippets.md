---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Contact = {
	emailAddresses : [
		{
			type : EmailType.Personal,
			name : "Pavel Bansky",
			address : "pavelb@adatum.onmicrosoft.com",
		},
		{
			address : "pavelb@fabrikam.onmicrosoft.com",
			name : "Pavel Bansky",
			type : EmailType.Other,
			otherLabel : "Volunteer work",
		},
	],
};

const result = async () => {
	await graphServiceClient.me.contactsById("contact-id").patch(requestBody);
}


```