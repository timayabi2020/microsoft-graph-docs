---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "return=representation",
		"If-Match": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
	}
};
const requestBody : PlannerTaskDetails = {
	previewType : PlannerPreviewType.NoPreview,
	references : {
		additionalData : {
			http%3A//developer%2Emicrosoft%2Ecom : {
				"@odata.type" : "microsoft.graph.plannerExternalReference",
				alias : "Documentation",
				previewPriority : " !",
				type : "Other",
			},
			"https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer" : {
				"@odata.type" : "microsoft.graph.plannerExternalReference",
				previewPriority : "  !!",
			},
			http%3A//www%2Ebing%2Ecom : null,
		},
	},
	checklist : {
		additionalData : {
			"95e27074-6c4a-447a-aa24-9d718a0b86fa" : {
				"@odata.type" : "microsoft.graph.plannerChecklistItem",
				title : "Update task details",
				isChecked : true,
			},
			"d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff" : {
				"@odata.type" : "microsoft.graph.plannerChecklistItem",
				isChecked : true,
			},
			"a93c93c5-10a6-4167-9551-8bafa09967a7" : null,
		},
	},
};

const result = async () => {
	await graphServiceClient.planner.tasksById("plannerTask-id").details.patch(requestBody, configuration);
}


```