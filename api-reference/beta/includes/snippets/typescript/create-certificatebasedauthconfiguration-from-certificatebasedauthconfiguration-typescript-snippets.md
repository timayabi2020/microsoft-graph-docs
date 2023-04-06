---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CertificateBasedAuthConfigurationPostRequestBody = {
	additionalData : {
		certificateAuthorities : [
			{
				isRootAuthority : true,
				certificate : "Binary",
			},
		],
	},
};

async () => {
	await graphServiceClient.organizationById("organization-id").certificateBasedAuthConfiguration.post(requestBody);
}


```