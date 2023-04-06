---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PhoneAuthenticationMethod = {
	phoneNumber : "+1 2065555554",
	phoneType : AuthenticationPhoneType.Mobile,
};

const result = async () => {
	await graphServiceClient.me.authentication.phoneMethodsById("phoneAuthenticationMethod-id").patch(requestBody);
}


```