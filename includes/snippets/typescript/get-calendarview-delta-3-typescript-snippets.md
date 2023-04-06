---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "odata.maxpagesize=2",
	}
,	queryParameters : {
		skiptoken: "R0usmci39OQxqJrxK4",
	}
};

const result = async () => {
	await graphServiceClient.me.calendarView.delta().get(configuration);
}


```