---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Contact = {
	homeAddress : {
		street : "123 Some street",
		city : "Seattle",
		state : "WA",
		postalCode : "98121",
	},
	birthday : new Date("1974-07-22"),
};

const result = async () => {
	await graphServiceClient.me.contactsById("contact-id").patch(requestBody);
}


```