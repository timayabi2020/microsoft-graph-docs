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
		startdatetime: "2016-12-01T00:00:00Z",
		enddatetime: "2016-12-30T00:00:00Z",
	}
};

const result = async () => {
	await graphServiceClient.me.calendarView.delta().get(configuration);
}


```