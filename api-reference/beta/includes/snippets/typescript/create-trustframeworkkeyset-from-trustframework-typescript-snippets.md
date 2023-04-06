---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TrustFrameworkKeySet = {
	id : "keyset1",
	keys : [
		{
			k : "k-value",
			x5c : [
				"x5c-value",
			],
			x5t : "x5t-value",
			kty : "kty-value",
			use : "use-value",
			exp : 99,
			nbf : 99,
			kid : "kid-value",
			e : "e-value",
			n : "n-value",
			d : "d-value",
			p : "p-value",
			q : "q-value",
			dp : "dp-value",
			dq : "dq-value",
			qi : "qi-value",
		},
	],
};

const result = async () => {
	await graphServiceClient.trustFramework.keySets.post(requestBody);
}


```