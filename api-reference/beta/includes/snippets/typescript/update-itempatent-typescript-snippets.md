---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemPatent = {
	number : "USPTO-3954432633",
	webUrl : "https://patents.gov/3954432633",
};

const result = async () => {
	await graphServiceClient.usersById("user-id").profile.patentsById("itemPatent-id").patch(requestBody);
}


```