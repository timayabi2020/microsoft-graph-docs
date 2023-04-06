---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemPhone = {
	type : PhoneType.Other,
};

const result = async () => {
	await graphServiceClient.usersById("user-id").profile.phonesById("itemPhone-id").patch(requestBody);
}


```