---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	keyCredentials : [
		{
			endDateTime : new Date("2024-01-11T15:31:26Z"),
			startDateTime : new Date("2023-01-12T15:31:26Z"),
			type : "AsymmetricX509Cert",
			usage : "Verify",
			key : "base64MIIDADCCAeigAwIBAgIQP6HEGDdZ65xJTcK4dCBvZzANBgkqhkiG9w0BAQsFADATMREwDwYDVQQDDAgyMDIzMDExMjAeFw0yMzAxMTIwODExNTZaFw0yNDAxMTIwODMxNTZaMBMxETAPBgNVBAMMCDIwMjMwMTEyMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAseKf1weEacJ67D6/...laxQPUbuIL+DaXVkKRm1V3GgIpKTBqMzTf4tCpy7rpUZbhcwAFw6h9A==",
			displayName : "CN=20230112",
		},
	],
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```