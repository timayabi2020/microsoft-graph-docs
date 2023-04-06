---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Team = {
	visibility : TeamVisibilityType.Private,
	displayName : "Sample Engineering Team",
	description : "This is a sample engineering team, used to showcase the range of properties supported by this API",
	channels : [
		{
			displayName : "Announcements 📢",
			isFavoriteByDefault : true,
			description : "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.",
		},
		{
			displayName : "Training 🏋️",
			isFavoriteByDefault : true,
			description : "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
			tabs : [
				{
					displayName : "A Pinned Website",
					configuration : {
						contentUrl : "https://learn.microsoft.com/microsoftteams/microsoft-teams",
					},
					additionalData : {
						"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
					},
				},
				{
					displayName : "A Pinned YouTube Video",
					configuration : {
						contentUrl : "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
						websiteUrl : "https://www.youtube.com/watch?v=X8krAMdGvCQ",
					},
					additionalData : {
						"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
					},
				},
			],
		},
		{
			displayName : "Planning 📅 ",
			description : "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
			isFavoriteByDefault : false,
		},
		{
			displayName : "Issues and Feedback 🐞",
			description : "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
		},
	],
	memberSettings : {
		allowCreateUpdateChannels : true,
		allowDeleteChannels : true,
		allowAddRemoveApps : true,
		allowCreateUpdateRemoveTabs : true,
		allowCreateUpdateRemoveConnectors : true,
	},
	guestSettings : {
		allowCreateUpdateChannels : false,
		allowDeleteChannels : false,
	},
	funSettings : {
		allowGiphy : true,
		giphyContentRating : GiphyRatingType.Moderate,
		allowStickersAndMemes : true,
		allowCustomMemes : true,
	},
	messagingSettings : {
		allowUserEditMessages : true,
		allowUserDeleteMessages : true,
		allowOwnerDeleteMessages : true,
		allowTeamMentions : true,
		allowChannelMentions : true,
	},
	installedApps : [
		{
			additionalData : {
				"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')",
			},
		},
		{
			additionalData : {
				"teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')",
			},
		},
	],
	additionalData : {
		"template@odata.bind" : "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
		discoverySettings : {
			showInTeamsSearchAndSuggestions : true,
		},
	},
};

const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```