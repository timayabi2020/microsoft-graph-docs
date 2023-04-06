---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrintConnector = {
	displayName : "ConnectorName",
	fullyQualifiedDomainName : "CONNECTOR-MACHINE",
	operatingSystem : "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
	appVersion : "0.19.7338.23496",
	location : {
		latitude : 1.1,
		longitude : 2.2,
		altitudeInMeters : 3,
	},
};

const result = async () => {
	await graphServiceClient.print.connectorsById("printConnector-id").patch(requestBody);
}


```