---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Contact = {
	givenName : "Pavel",
	surname : "Bansky",
	emailAddresses : [
		{
			address : "pavelb@contoso.onmicrosoft.com",
			name : "Pavel Bansky",
			type : EmailType.Personal,
		},
		{
			address : "pavelb@fabrikam.onmicrosoft.com",
			name : "Pavel Bansky",
			type : EmailType.Other,
			otherLabel : "Volunteer work",
		},
	],
	phones : [
		{
			number : "+1 732 555 0102",
			type : PhoneType.Business,
		},
	],
};

const result = async () => {
	await graphServiceClient.me.contacts.post(requestBody);
}


```