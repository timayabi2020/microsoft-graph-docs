---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingBusiness = {
	displayName : "Fourth Coffee",
	address : {
		street : "4567 Main Street",
		city : "Buffalo",
		state : "NY",
		countryOrRegion : "USA",
		postalCode : "98052",
		additionalData : {
			"postOfficeBox" : "P.O. Box 123",
		},
	},
	phone : "206-555-0100",
	email : "manager@fourthcoffee.com",
	webSiteUrl : "https://www.fourthcoffee.com",
	defaultCurrencyIso : "USD",
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinesses.post(requestBody);
}


```