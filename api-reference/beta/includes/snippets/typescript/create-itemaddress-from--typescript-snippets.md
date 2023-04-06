---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemAddress = {
	displayName : "Home",
	detail : {
		type : PhysicalAddressType.Home,
		postOfficeBox : null,
		street : "221B Baker Street",
		city : "London",
		state : null,
		countryOrRegion : "United Kingdom",
		postalCode : "E14 3TD",
	},
};

const result = async () => {
	await graphServiceClient.me.profile.addresses.post(requestBody);
}


```