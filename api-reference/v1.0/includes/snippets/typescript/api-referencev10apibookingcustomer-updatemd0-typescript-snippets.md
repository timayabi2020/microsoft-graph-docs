---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingCustomerBase = {
	"@odata.type" : "#microsoft.graph.bookingCustomer",
	additionalData : {
		"displayName" : "Adele",
		"emailAddress" : "adele@relecloud.com",
	},
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinessesById("bookingBusiness-id").customersById("bookingCustomerBase-id").patch(requestBody);
}


```