---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LogTeleconferenceDeviceQualityPostRequestBody = {
	quality : {
		"@odata.type" : "#microsoft.graph.teleconferenceDeviceQuality",
		callChainId : "0622673d-9f69-49b3-9d4f-5ec64f42ecce",
		participantId : "ea078406-b5d4-4d3c-b85e-90103dcec7f6",
		mediaLegId : "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f",
		deviceName : "TestAgent",
		deviceDescription : "TestDescription",
		mediaQualityList : [
			{
				"@odata.type" : "#microsoft.graph.teleconferenceDeviceAudioQuality",
				channelIndex : 1,
				mediaDuration : pT20M,
				networkLinkSpeedInBytes : 13000,
				localIPAddress : "127.0.0.1",
				localPort : 6300,
				remoteIPAddress : "102.1.1.101",
				remotePort : 6301,
				inboundPackets : 5500,
				outboundPackets : 5400,
				averageInboundPacketLossRateInPercentage : 0.01,
				averageOutboundPacketLossRateInPercentage : 0.02,
				maximumInboundPacketLossRateInPercentage : 0.05,
				maximumOutboundPacketLossRateInPercentage : 0.06,
				averageInboundRoundTripDelay : pT0.03S,
				averageOutboundRoundTripDelay : pT0.04S,
				maximumInboundRoundTripDelay : pT0.13S,
				maximumOutboundRoundTripDelay : pT0.14S,
				averageInboundJitter : pT0.01S,
				averageOutboundJitter : pT0.015S,
				maximumInboundJitter : pT0.023S,
				maximumOutboundJitter : pT0.024S,
			},
			{
				"@odata.type" : "#microsoft.graph.teleconferenceDeviceVideoQuality",
				channelIndex : 1,
				mediaDuration : pT20M,
				networkLinkSpeedInBytes : 13000,
				localIPAddress : "127.0.0.1",
				localPort : 6300,
				remoteIPAddress : "102.1.1.101",
				remotePort : 6301,
				inboundPackets : 5500,
				outboundPackets : 5400,
				averageInboundPacketLossRateInPercentage : 0.01,
				averageOutboundPacketLossRateInPercentage : 0.02,
				maximumInboundPacketLossRateInPercentage : 0.05,
				maximumOutboundPacketLossRateInPercentage : 0.06,
				averageInboundRoundTripDelay : pT0.03S,
				averageOutboundRoundTripDelay : pT0.04S,
				maximumInboundRoundTripDelay : pT0.13S,
				maximumOutboundRoundTripDelay : pT0.14S,
				averageInboundJitter : pT0.01S,
				averageOutboundJitter : pT0.015S,
				maximumInboundJitter : pT0.023S,
				maximumOutboundJitter : pT0.024S,
			},
			{
				"@odata.type" : "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
				channelIndex : 1,
				mediaDuration : pT20M,
				networkLinkSpeedInBytes : 13000,
				localIPAddress : "127.0.0.1",
				localPort : 6300,
				remoteIPAddress : "102.1.1.101",
				remotePort : 6301,
				inboundPackets : 5500,
				outboundPackets : 5400,
				averageInboundPacketLossRateInPercentage : 0.01,
				averageOutboundPacketLossRateInPercentage : 0.02,
				maximumInboundPacketLossRateInPercentage : 0.05,
				maximumOutboundPacketLossRateInPercentage : 0.06,
				averageInboundRoundTripDelay : pT0.03S,
				averageOutboundRoundTripDelay : pT0.04S,
				maximumInboundRoundTripDelay : pT0.13S,
				maximumOutboundRoundTripDelay : pT0.14S,
				averageInboundJitter : pT0.01S,
				averageOutboundJitter : pT0.015S,
				maximumInboundJitter : pT0.023S,
				maximumOutboundJitter : pT0.024S,
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.communications.calls.logTeleconferenceDeviceQuality.post(requestBody);
}


```