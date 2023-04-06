---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonAnnualEvent = {
	type : PersonAnnualEventType.Birthday,
	date : "1980-01-08",
};

const result = async () => {
	await graphServiceClient.me.profile.anniversaries.post(requestBody);
}


```