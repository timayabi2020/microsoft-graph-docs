---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "microsoft.graph.countryNamedLocation/countriesAndRegions/any",
	}
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocations.get(configuration);
}


```