---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RegionalAndLanguageSettingsPutRequestBody = {
	additionalData : {
		defaultDisplayLanguage : {
			locale : "en-US",
		},
		authoringLanguages : [
			{
				locale : "fr-FR",
			},
			{
				locale : "de-DE",
			},
		],
		defaultTranslationLanguage : {
			locale : "en-US",
		},
		defaultSpeechInputLanguage : {
			locale : "en-US",
		},
		defaultRegionalFormat : {
			locale : "en-GB",
		},
		regionalFormatOverrides : {
			calendar : "Gregorian Calendar",
			firstDayOfWeek : "Sunday",
			shortDateFormat : "yyyy-MM-dd",
			longDateFormat : "dddd, MMMM d, yyyy",
			shortTimeFormat : "HH:mm",
			longTimeFormat : "h:mm:ss tt",
			timeZone : "Pacific Standard Time",
		},
		translationPreferences : {
			translationBehavior : "Yes",
			languageOverrides : [
				{
					languageTag : "fr",
					translationBehavior : "Yes",
				},
			],
		},
	},
};

async () => {
	await graphServiceClient.me.settings.regionalAndLanguageSettings.put(requestBody);
}


```