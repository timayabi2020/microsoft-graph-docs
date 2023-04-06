---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NamedLocation = {
	"@odata.type" : "#microsoft.graph.ipNamedLocation",
	displayName : "Untrusted IP named location",
	additionalData : {
		isTrusted : false,
		ipRanges : [
			{
				"@odata.type" : "#microsoft.graph.iPv4CidrRange",
				cidrAddress : "12.34.221.11/22",
			},
			{
				"@odata.type" : "#microsoft.graph.iPv6CidrRange",
				cidrAddress : "2001:0:9d38:90d6:0:0:0:0/63",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocations.post(requestBody);
}


```