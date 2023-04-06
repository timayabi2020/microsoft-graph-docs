---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemPatent = {
	description : "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
	displayName : "Inferring User Intent through browsing behaviors",
	isPending : true,
	number : "USPTO-3954432633",
	webUrl : "https://patents.gov/3954432633",
};

const result = async () => {
	await graphServiceClient.me.profile.patents.post(requestBody);
}


```