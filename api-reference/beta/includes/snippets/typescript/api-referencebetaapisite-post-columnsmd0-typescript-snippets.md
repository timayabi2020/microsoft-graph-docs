---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ColumnDefinition = {
	description : "test",
	enforceUniqueValues : false,
	hidden : false,
	indexed : false,
	name : "Title",
	text : {
		allowMultipleLines : false,
		appendChangesToExistingText : false,
		linesForEditing : 0,
		maxLength : 255,
	},
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").columns.post(requestBody);
}


```