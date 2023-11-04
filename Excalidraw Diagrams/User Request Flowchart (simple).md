---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Cilium
Ingress Controller ^WeCAT4KR

Ambassador
API Gateway ^IkV1RQHq

1. User Request via
    Website UI or CLI ^BQcoz1hD

3. NGINX (SSL/TLS)
    HAProxy (Load Balance) ^X735tFNz

3a. Cilium Ingress Controller ^oFr5B16K

3b. ^XwxIQK04

NGINX ^beTkFd4I

HAProxy ^wRx3IT9J

NGINX ^VpUhjJxy

HAProxy ^Gc2a3svu

NGINX ^tqChK8S7

HAProxy ^UNUdZoP7

Autoscaling Groups
(per region) ^qViXnrhp

2. AWS Route53
(Global Server Load Balancing) ^G7PCYfkM

Route53 ^N3tNI5bf

1. Ingress Rules: 
The Ingress Controller evaluates the 
Ingress rules that define how external requests should 
be routed to internal microservices. These rules specify 
the path, host, and other routing conditions. ^0BZQmdDq

2. Service Discovery:
The Cilium Ingress Controller uses service discovery to 
identify the appropriate microservice or destination within
your Cilium Service Mesh based on the defined Ingress rules. ^73GM9ZUt

3. Routing and Load Balancing: 
If multiple instances of the microservice are available, 
Cilium Service Mesh provides load balancing. The Ingress Controller
routes the request to one of the available instances. ^Zah8zWpE

4. Security and Policy Enforcement:
As the request enters the Cilium Service Mesh, Cilium enforces security and 
policy rules such as network segmentation, authentication, and authorization. ^KjmOloik

5. Microservice Execution: 
The request is forwarded to the appropriate 
microservice instance within the Service Mesh. ^L9AN7WoI

6. Response Generation: 
The microservice processes the request and generates a response. ^IQwdIMaG

7. Response Back to User: 
The response is then sent back through the Cilium Ingress Controller, 
which ensures it's properly routed back to the user who initiated the request. ^rDlzX7Vw

1. Ambassador API Gateway Processing:
The Ambassador API Gateway receives the request and processes it. 
This processing may include tasks like routing to specific microservices, 
authentication, and applying routing policies. ^MYlA5SPL

3. Microservice Access: 
Depending on the configuration and routing rules in the 
Ambassador API Gateway, the request may be further routed 
to one or more internal microservices within your Kubernetes cluster. ^Q0nNSnSl

2. Security and Policy Enforcement: 
The Ambassador API Gateway enforces security and policy rules, 
such as access control and rate limiting, to protect the microservices. ^SBoK0dve

4. Microservice Execution: 
The request reaches the appropriate microservice within your 
Kubernetes cluster, and the microservice processes the request. ^TuZXv707

5. Response Generation: 
The microservice processes the request and generates a 
response, which is then sent back to the Ambassador API Gateway. ^qY5gJ7In

6. Response Back to User: 
The Ambassador API Gateway ensures that the response
is properly routed back to the user who initiated the request. ^Qw1Z7msL

API Gateway ^0E0F5ZMW

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.27",
	"elements": [
		{
			"type": "rectangle",
			"version": 804,
			"versionNonce": 145424797,
			"isDeleted": false,
			"id": "zMuumi43h2siyC_NZMhGV",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1394.5729965498708,
			"y": -626.3484124275972,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 432.3838657309797,
			"height": 190.95125034819915,
			"seed": 164560531,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "WeCAT4KR"
				}
			],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"customData": {
				"legacyTextWrap": true
			}
		},
		{
			"type": "text",
			"version": 957,
			"versionNonce": 1249035773,
			"isDeleted": false,
			"id": "WeCAT4KR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1434.1794191614545,
			"y": -582.3465756675026,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 353.1710205078125,
			"height": 102.94757682801003,
			"seed": 1874248435,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 44.75981601217828,
			"fontFamily": 2,
			"text": "Cilium\nIngress Controller",
			"rawText": "Cilium\nIngress Controller",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "zMuumi43h2siyC_NZMhGV",
			"originalText": "Cilium\nIngress Controller",
			"lineHeight": 1.15,
			"baseline": 92
		},
		{
			"type": "rectangle",
			"version": 1055,
			"versionNonce": 1595623106,
			"isDeleted": false,
			"id": "yF8hb1OMpkb7MXKbK0Pih",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1412.1581829930337,
			"y": 262.4708955855218,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 434.578707689005,
			"height": 208.50998601240138,
			"seed": 1917209117,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "IkV1RQHq"
				}
			],
			"updated": 1699094033380,
			"link": null,
			"locked": false,
			"customData": {
				"legacyTextWrap": true
			}
		},
		{
			"type": "text",
			"version": 1242,
			"versionNonce": 1732845186,
			"isDeleted": false,
			"id": "IkV1RQHq",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1498.8684352750363,
			"y": 315.25737902548036,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 261.158203125,
			"height": 102.93701913248427,
			"seed": 1940959795,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1699094033381,
			"link": null,
			"locked": false,
			"fontSize": 44.75522570977577,
			"fontFamily": 2,
			"text": "Ambassador\nAPI Gateway",
			"rawText": "Ambassador\nAPI Gateway",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "yF8hb1OMpkb7MXKbK0Pih",
			"originalText": "Ambassador\nAPI Gateway",
			"lineHeight": 1.15,
			"baseline": 92
		},
		{
			"type": "ellipse",
			"version": 237,
			"versionNonce": 814926621,
			"isDeleted": false,
			"id": "WPETSZ1m1RSkhhYytdPOg",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2174.1641169888026,
			"y": -342.88413415980995,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 139.92933710538503,
			"height": 124.36817282631151,
			"seed": 2082283261,
			"groupIds": [
				"pCrOB6FIhn_hBeePU1ck1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 202,
			"versionNonce": 94723965,
			"isDeleted": false,
			"id": "9rDAfbfn-52Je-KauNrWQ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2103.393555067937,
			"y": -217.3081313360001,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 2.208826846247808,
			"height": 217.15427926699533,
			"seed": 549407795,
			"groupIds": [
				"pCrOB6FIhn_hBeePU1ck1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.208826846247808,
					217.15427926699533
				]
			]
		},
		{
			"type": "line",
			"version": 243,
			"versionNonce": 1478911965,
			"isDeleted": false,
			"id": "qDHNaeQEztl8fvUQYZE7W",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2194.2859717472343,
			"y": -155.37398460212148,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 176.03312540611492,
			"height": 0.956163450406942,
			"seed": 1119241213,
			"groupIds": [
				"pCrOB6FIhn_hBeePU1ck1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					176.03312540611492,
					0.956163450406942
				]
			]
		},
		{
			"type": "line",
			"version": 219,
			"versionNonce": 1512531005,
			"isDeleted": false,
			"id": "myayqM57iNiwGCf4kCjaa",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2102.2899236226913,
			"y": 0.618383667998387,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 62.28844787746621,
			"height": 71.5343262308551,
			"seed": 346840733,
			"groupIds": [
				"pCrOB6FIhn_hBeePU1ck1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-62.28844787746621,
					71.5343262308551
				]
			]
		},
		{
			"type": "line",
			"version": 291,
			"versionNonce": 2139739293,
			"isDeleted": false,
			"id": "Rn21wcc9pq5VHzrM2kXwz",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2100.444682768835,
			"y": 0.41319107950880607,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 62.28844787746621,
			"height": 71.5343262308551,
			"seed": 1532353533,
			"groupIds": [
				"pCrOB6FIhn_hBeePU1ck1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					62.28844787746621,
					71.5343262308551
				]
			]
		},
		{
			"type": "text",
			"version": 389,
			"versionNonce": 832829501,
			"isDeleted": false,
			"id": "BQcoz1hD",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1979.0294053819453,
			"y": -1631.0413430179617,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 663.352294921875,
			"height": 169.81783657796086,
			"seed": 1836336083,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "1. User Request via\n    Website UI or CLI",
			"rawText": "1. User Request via\n    Website UI or CLI",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1. User Request via\n    Website UI or CLI",
			"lineHeight": 1.15,
			"baseline": 152
		},
		{
			"type": "arrow",
			"version": 210,
			"versionNonce": 1649666205,
			"isDeleted": false,
			"id": "XbKL_Qs4lcbWwX3hZfPPF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -953.0973665135448,
			"y": -1542.6470545614593,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 740.0403471497297,
			"height": 2.856657986065913,
			"seed": 921375357,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					740.0403471497297,
					-2.856657986065913
				]
			]
		},
		{
			"type": "text",
			"version": 621,
			"versionNonce": 1818676477,
			"isDeleted": false,
			"id": "X735tFNz",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2037.9671855355919,
			"y": -1666.3430971469265,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 894.5758666992188,
			"height": 169.81783657796086,
			"seed": 1615534131,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "3. NGINX (SSL/TLS)\n    HAProxy (Load Balance)",
			"rawText": "3. NGINX (SSL/TLS)\n    HAProxy (Load Balance)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3. NGINX (SSL/TLS)\n    HAProxy (Load Balance)",
			"lineHeight": 1.15,
			"baseline": 152
		},
		{
			"type": "arrow",
			"version": 474,
			"versionNonce": 257828189,
			"isDeleted": false,
			"id": "eoMHcymdps5hpzISh4lrd",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3103.6694858095043,
			"y": -1624.6690489211226,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 812.3644763972521,
			"height": 346.66227816440687,
			"seed": 1663754259,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					812.3644763972521,
					-346.66227816440687
				]
			]
		},
		{
			"type": "text",
			"version": 735,
			"versionNonce": 512455101,
			"isDeleted": false,
			"id": "oFr5B16K",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4028.1932054617146,
			"y": -2053.656962859327,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 931.418701171875,
			"height": 84.90891828898043,
			"seed": 1635851933,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "3a. Cilium Ingress Controller",
			"rawText": "3a. Cilium Ingress Controller",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3a. Cilium Ingress Controller",
			"lineHeight": 1.15,
			"baseline": 68
		},
		{
			"type": "arrow",
			"version": 599,
			"versionNonce": 118501917,
			"isDeleted": false,
			"id": "eReyvqhKyxxVRO9wg8FNi",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 3.141592653589793,
			"x": 3930.747948318991,
			"y": -1203.212435531255,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 812.3644763972521,
			"height": 346.66227816440687,
			"seed": 335673043,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-812.3644763972521,
					-346.66227816440687
				]
			]
		},
		{
			"type": "text",
			"version": 809,
			"versionNonce": 1347479042,
			"isDeleted": false,
			"id": "XwxIQK04",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4010.758300845847,
			"y": -1250.131311105193,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 102.6337890625,
			"height": 84.90891828898043,
			"seed": 509334493,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1699094038402,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "3b.",
			"rawText": "3b.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3b.",
			"lineHeight": 1.15,
			"baseline": 68
		},
		{
			"type": "arrow",
			"version": 262,
			"versionNonce": 1140799741,
			"isDeleted": false,
			"id": "WFEPMA2Fn6po7WOVzpyvB",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1819.1814152000343,
			"y": -101.4475751216545,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 302.1490694736584,
			"height": 1.199177557087878,
			"seed": 1332160541,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					302.1490694736584,
					1.199177557087878
				]
			]
		},
		{
			"type": "rectangle",
			"version": 737,
			"versionNonce": 822677853,
			"isDeleted": false,
			"id": "__0pQtV_SIHh821bXnNmE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -246.95139840142383,
			"y": -852.0171075804631,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 905.5714511218281,
			"height": 1540.0354003906255,
			"seed": 314074749,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 509,
			"versionNonce": 603512253,
			"isDeleted": false,
			"id": "Ath9RiVSXt1ogl68XGnXO",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -141.1323562884254,
			"y": -588.791327292802,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 683.1178019021356,
			"height": 343.14927018219527,
			"seed": 350262237,
			"groupIds": [
				"S1qu5dqM4cdvvqOWHWQWZ"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 522,
			"versionNonce": 1408245277,
			"isDeleted": false,
			"id": "fJ5NBtzc2dlIud71vjn6f",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 189.97619230014857,
			"y": -583.0204029580229,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 2.7910528196847797,
			"height": 342.79780008814777,
			"seed": 1287356979,
			"groupIds": [
				"S1qu5dqM4cdvvqOWHWQWZ"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-2.7910528196847797,
					342.79780008814777
				]
			]
		},
		{
			"type": "arrow",
			"version": 647,
			"versionNonce": 400577149,
			"isDeleted": false,
			"id": "fTMYcWMroJUOEj_uOHXWA",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 130.50376261017823,
			"y": -414.3219114646006,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 124.64142341094438,
			"height": 2.3294764547057674,
			"seed": 1359365043,
			"groupIds": [
				"S1qu5dqM4cdvvqOWHWQWZ"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					124.64142341094438,
					-2.3294764547057674
				]
			]
		},
		{
			"type": "text",
			"version": 579,
			"versionNonce": 1821047517,
			"isDeleted": false,
			"id": "beTkFd4I",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -69.33155299427835,
			"y": -443.17378463106525,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 158.22288513183594,
			"height": 57.46148611084624,
			"seed": 493172381,
			"groupIds": [
				"S1qu5dqM4cdvvqOWHWQWZ"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "NGINX",
			"rawText": "NGINX",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "NGINX",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "text",
			"version": 654,
			"versionNonce": 981571389,
			"isDeleted": false,
			"id": "wRx3IT9J",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 277.62903102618816,
			"y": -444.5749398335224,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 197.10777282714844,
			"height": 57.46148611084624,
			"seed": 1040311229,
			"groupIds": [
				"S1qu5dqM4cdvvqOWHWQWZ"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "HAProxy",
			"rawText": "HAProxy",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "HAProxy",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "rectangle",
			"version": 503,
			"versionNonce": 1545971613,
			"isDeleted": false,
			"id": "j2Q_-Uleo3d2eknXP380r",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -148.5322419107215,
			"y": -180.7195415220167,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 683.1178019021356,
			"height": 343.14927018219527,
			"seed": 1574880915,
			"groupIds": [
				"JxyN6iD_HzaMhSeWAxj1e"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 516,
			"versionNonce": 1671998461,
			"isDeleted": false,
			"id": "soiUFFx5uxReg1UOtkRnU",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 182.57630667785247,
			"y": -174.9486171872377,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 2.7910528196847797,
			"height": 342.79780008814777,
			"seed": 155508765,
			"groupIds": [
				"JxyN6iD_HzaMhSeWAxj1e"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-2.7910528196847797,
					342.79780008814777
				]
			]
		},
		{
			"type": "arrow",
			"version": 641,
			"versionNonce": 554443869,
			"isDeleted": false,
			"id": "VK7IAAHRpDr8muddEgHIJ",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 123.10387698788213,
			"y": -6.250125693815335,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 124.64142341094438,
			"height": 2.3294764547057674,
			"seed": 1108245555,
			"groupIds": [
				"JxyN6iD_HzaMhSeWAxj1e"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					124.64142341094438,
					-2.3294764547057674
				]
			]
		},
		{
			"type": "text",
			"version": 573,
			"versionNonce": 1747030205,
			"isDeleted": false,
			"id": "VpUhjJxy",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -76.73143861657445,
			"y": -35.10199886027988,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 158.22288513183594,
			"height": 57.46148611084624,
			"seed": 156030077,
			"groupIds": [
				"JxyN6iD_HzaMhSeWAxj1e"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "NGINX",
			"rawText": "NGINX",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "NGINX",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "text",
			"version": 648,
			"versionNonce": 378171677,
			"isDeleted": false,
			"id": "Gc2a3svu",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 270.22914540389206,
			"y": -36.50315406273705,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 197.10777282714844,
			"height": 57.46148611084624,
			"seed": 502693331,
			"groupIds": [
				"JxyN6iD_HzaMhSeWAxj1e"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "HAProxy",
			"rawText": "HAProxy",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "HAProxy",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "rectangle",
			"version": 549,
			"versionNonce": 1505248637,
			"isDeleted": false,
			"id": "ixP-o0w2Urm-MFNIU0UE0",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -144.5563188329029,
			"y": 244.20686091199207,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 683.1178019021356,
			"height": 343.14927018219527,
			"seed": 1092041949,
			"groupIds": [
				"Q2Vav75XSN-O1JaXGAvjr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 562,
			"versionNonce": 887918045,
			"isDeleted": false,
			"id": "zlLj4fXaazTCERAdk8Tcb",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 186.55222975567108,
			"y": 249.97778524677108,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 2.7910528196847797,
			"height": 342.79780008814777,
			"seed": 1823296371,
			"groupIds": [
				"Q2Vav75XSN-O1JaXGAvjr"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-2.7910528196847797,
					342.79780008814777
				]
			]
		},
		{
			"type": "arrow",
			"version": 687,
			"versionNonce": 1194904125,
			"isDeleted": false,
			"id": "6dH80t4oqeg6cZmYlhOIu",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 127.07980006570074,
			"y": 418.6762767401934,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 124.64142341094438,
			"height": 2.3294764547057674,
			"seed": 2016778557,
			"groupIds": [
				"Q2Vav75XSN-O1JaXGAvjr"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					124.64142341094438,
					-2.3294764547057674
				]
			]
		},
		{
			"type": "text",
			"version": 619,
			"versionNonce": 1367243421,
			"isDeleted": false,
			"id": "tqChK8S7",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -72.75551553875584,
			"y": 389.8244035737289,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 158.22288513183594,
			"height": 57.46148611084624,
			"seed": 41510163,
			"groupIds": [
				"Q2Vav75XSN-O1JaXGAvjr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "NGINX",
			"rawText": "NGINX",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "NGINX",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "text",
			"version": 694,
			"versionNonce": 2087657213,
			"isDeleted": false,
			"id": "UNUdZoP7",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 274.20506848171067,
			"y": 388.42324837127165,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 197.10777282714844,
			"height": 57.46148611084624,
			"seed": 134834589,
			"groupIds": [
				"Q2Vav75XSN-O1JaXGAvjr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "HAProxy",
			"rawText": "HAProxy",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "HAProxy",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "text",
			"version": 693,
			"versionNonce": 1586247517,
			"isDeleted": false,
			"id": "qViXnrhp",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -87.33239412595572,
			"y": -796.5854920992267,
			"strokeColor": "#000000",
			"backgroundColor": "#228be6",
			"width": 569.0909423828125,
			"height": 149.98369373490388,
			"seed": 1113676477,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 65.21030162387126,
			"fontFamily": 2,
			"text": "Autoscaling Groups\n(per region)",
			"rawText": "Autoscaling Groups\n(per region)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Autoscaling Groups\n(per region)",
			"lineHeight": 1.15,
			"baseline": 135
		},
		{
			"type": "text",
			"version": 684,
			"versionNonce": 2109083357,
			"isDeleted": false,
			"id": "G7PCYfkM",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -72.14599127726274,
			"y": -1626.5503825921064,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 1030.087158203125,
			"height": 169.81783657796086,
			"seed": 1507753469,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "2. AWS Route53\n(Global Server Load Balancing)",
			"rawText": "2. AWS Route53\n(Global Server Load Balancing)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2. AWS Route53\n(Global Server Load Balancing)",
			"lineHeight": 1.15,
			"baseline": 152
		},
		{
			"type": "arrow",
			"version": 265,
			"versionNonce": 489302845,
			"isDeleted": false,
			"id": "VGHGbeOa7nXX9Kpe8MhPP",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1040.8942744887681,
			"y": -1545.97724236342,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 740.0403471497297,
			"height": 2.856657986065913,
			"seed": 1194177843,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963506123,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					740.0403471497297,
					-2.856657986065913
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1098,
			"versionNonce": 1109869501,
			"isDeleted": false,
			"id": "2b434f5RGdxzFjYNfcX9I",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1407.4632918118864,
			"y": -185.81572885084427,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 381.68861547059703,
			"height": 183.21053542588658,
			"seed": 321807805,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "N3tNI5bf"
				}
			],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"customData": {
				"legacyTextWrap": true
			}
		},
		{
			"type": "text",
			"version": 360,
			"versionNonce": 727827485,
			"isDeleted": false,
			"id": "N3tNI5bf",
			"fillStyle": "solid",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1311.0623968573495,
			"y": -122.9412041933241,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 188.88682556152344,
			"height": 57.46148611084624,
			"seed": 2040116541,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"fontSize": 49.96650966160543,
			"fontFamily": 2,
			"text": "Route53",
			"rawText": "Route53",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "2b434f5RGdxzFjYNfcX9I",
			"originalText": "Route53",
			"lineHeight": 1.15,
			"baseline": 46
		},
		{
			"type": "arrow",
			"version": 438,
			"versionNonce": 506280061,
			"isDeleted": false,
			"id": "VQPoutr2hcMEDYSVfdK7F",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -889.5995343498716,
			"y": -39.4404561404117,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 543.1656860707841,
			"height": 5.908161452379213,
			"seed": 79317363,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					543.1656860707841,
					5.908161452379213
				]
			]
		},
		{
			"type": "arrow",
			"version": 478,
			"versionNonce": 608903389,
			"isDeleted": false,
			"id": "OVXX3Iudb9YT0bZz_wHVE",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -883.0190611140802,
			"y": -179.81824623289572,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 547.3212034012655,
			"height": 194.08585221811023,
			"seed": 1285325981,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					547.3212034012655,
					-194.08585221811023
				]
			]
		},
		{
			"type": "arrow",
			"version": 599,
			"versionNonce": 323812669,
			"isDeleted": false,
			"id": "sQuLt_obhnG6vK8M_Aagn",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 3.141592653589793,
			"x": -332.87716726136705,
			"y": 341.6606647858871,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 553.1664880398213,
			"height": 257.5594310130029,
			"seed": 758544029,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-553.1664880398213,
					-257.5594310130029
				]
			]
		},
		{
			"type": "arrow",
			"version": 139,
			"versionNonce": 311709085,
			"isDeleted": false,
			"id": "0iSNi00U_TT9k1v3ccvUV",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 751.1242706171133,
			"y": -25.420793630872936,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 558.4500229404861,
			"height": 448.17265704479655,
			"seed": 1606981843,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					558.4500229404861,
					-448.17265704479655
				]
			]
		},
		{
			"type": "arrow",
			"version": 205,
			"versionNonce": 1632801277,
			"isDeleted": false,
			"id": "Vj-qcadyRhT-j2dC4S8vS",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 3.141592653589793,
			"x": 1307.8688275555114,
			"y": 344.7910815293334,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 555.2585540040158,
			"height": 299.43077679931366,
			"seed": 1553142483,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698963513241,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-555.2585540040158,
					-299.43077679931366
				]
			]
		},
		{
			"type": "rectangle",
			"version": 270,
			"versionNonce": 1626897299,
			"isDeleted": false,
			"id": "N32GT1dzYlHyW3s5YKmNX",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2078.9463345966647,
			"y": -907.8125918508318,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 2662.2745768229174,
			"height": 922.0398966471366,
			"seed": 669237619,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 419,
			"versionNonce": 629996317,
			"isDeleted": false,
			"id": "0BZQmdDq",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2181.3458271329387,
			"y": -834.7922729566726,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 890.384765625,
			"height": 207,
			"seed": 828749533,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "1. Ingress Rules: \nThe Ingress Controller evaluates the \nIngress rules that define how external requests should \nbe routed to internal microservices. These rules specify \nthe path, host, and other routing conditions.",
			"rawText": "1. Ingress Rules: \nThe Ingress Controller evaluates the \nIngress rules that define how external requests should \nbe routed to internal microservices. These rules specify \nthe path, host, and other routing conditions.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1. Ingress Rules: \nThe Ingress Controller evaluates the \nIngress rules that define how external requests should \nbe routed to internal microservices. These rules specify \nthe path, host, and other routing conditions.",
			"lineHeight": 1.15,
			"baseline": 198
		},
		{
			"type": "text",
			"version": 204,
			"versionNonce": 36278579,
			"isDeleted": false,
			"id": "73GM9ZUt",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2177.679369729665,
			"y": -532.5217695038268,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 980.490234375,
			"height": 165.6,
			"seed": 1243312499,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "2. Service Discovery:\nThe Cilium Ingress Controller uses service discovery to \nidentify the appropriate microservice or destination within\nyour Cilium Service Mesh based on the defined Ingress rules.",
			"rawText": "2. Service Discovery:\nThe Cilium Ingress Controller uses service discovery to \nidentify the appropriate microservice or destination within\nyour Cilium Service Mesh based on the defined Ingress rules.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2. Service Discovery:\nThe Cilium Ingress Controller uses service discovery to \nidentify the appropriate microservice or destination within\nyour Cilium Service Mesh based on the defined Ingress rules.",
			"lineHeight": 1.15,
			"baseline": 157
		},
		{
			"type": "text",
			"version": 263,
			"versionNonce": 1004113789,
			"isDeleted": false,
			"id": "Zah8zWpE",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2187.202487521704,
			"y": -255.11937198475982,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 1092.498046875,
			"height": 165.6,
			"seed": 212128573,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "3. Routing and Load Balancing: \nIf multiple instances of the microservice are available, \nCilium Service Mesh provides load balancing. The Ingress Controller\nroutes the request to one of the available instances.",
			"rawText": "3. Routing and Load Balancing: \nIf multiple instances of the microservice are available, \nCilium Service Mesh provides load balancing. The Ingress Controller\nroutes the request to one of the available instances.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3. Routing and Load Balancing: \nIf multiple instances of the microservice are available, \nCilium Service Mesh provides load balancing. The Ingress Controller\nroutes the request to one of the available instances.",
			"lineHeight": 1.15,
			"baseline": 157
		},
		{
			"type": "text",
			"version": 300,
			"versionNonce": 870773459,
			"isDeleted": false,
			"id": "KjmOloik",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3449.9125705295164,
			"y": -803.6821364704374,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 1226.724609375,
			"height": 124.19999999999999,
			"seed": 456313619,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "4. Security and Policy Enforcement:\nAs the request enters the Cilium Service Mesh, Cilium enforces security and \npolicy rules such as network segmentation, authentication, and authorization.",
			"rawText": "4. Security and Policy Enforcement:\nAs the request enters the Cilium Service Mesh, Cilium enforces security and \npolicy rules such as network segmentation, authentication, and authorization.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "4. Security and Policy Enforcement:\nAs the request enters the Cilium Service Mesh, Cilium enforces security and \npolicy rules such as network segmentation, authentication, and authorization.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 349,
			"versionNonce": 408197085,
			"isDeleted": false,
			"id": "L9AN7WoI",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3457.3482801649334,
			"y": -562.2383905394479,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 746.279296875,
			"height": 124.19999999999999,
			"seed": 2122408861,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "5. Microservice Execution: \nThe request is forwarded to the appropriate \nmicroservice instance within the Service Mesh.",
			"rawText": "5. Microservice Execution: \nThe request is forwarded to the appropriate \nmicroservice instance within the Service Mesh.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "5. Microservice Execution: \nThe request is forwarded to the appropriate \nmicroservice instance within the Service Mesh.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 270,
			"versionNonce": 919019635,
			"isDeleted": false,
			"id": "IQwdIMaG",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3455.9643283420164,
			"y": -355.44704939361463,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 1076.572265625,
			"height": 82.8,
			"seed": 795734195,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "6. Response Generation: \nThe microservice processes the request and generates a response.",
			"rawText": "6. Response Generation: \nThe microservice processes the request and generates a response.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "6. Response Generation: \nThe microservice processes the request and generates a response.",
			"lineHeight": 1.15,
			"baseline": 74
		},
		{
			"type": "text",
			"version": 276,
			"versionNonce": 1427084349,
			"isDeleted": false,
			"id": "rDlzX7Vw",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3446.2613661024334,
			"y": -187.80569197173986,
			"strokeColor": "#000000",
			"backgroundColor": "#f40b5d",
			"width": 1211.537109375,
			"height": 124.19999999999999,
			"seed": 992798717,
			"groupIds": [
				"Imze4qKYeOW0Iovu8MpZI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277570971,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "7. Response Back to User: \nThe response is then sent back through the Cilium Ingress Controller, \nwhich ensures it's properly routed back to the user who initiated the request.",
			"rawText": "7. Response Back to User: \nThe response is then sent back through the Cilium Ingress Controller, \nwhich ensures it's properly routed back to the user who initiated the request.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "7. Response Back to User: \nThe response is then sent back through the Cilium Ingress Controller, \nwhich ensures it's properly routed back to the user who initiated the request.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "rectangle",
			"version": 899,
			"versionNonce": 1877095859,
			"isDeleted": false,
			"id": "wZjwd3qEEZgGrA4RBY0BP",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2098.395960247707,
			"y": 136.06209280086205,
			"strokeColor": "#000000",
			"backgroundColor": "#a089e6",
			"width": 2470.997721354168,
			"height": 744.8538614908862,
			"seed": 1513742259,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 516649725,
			"isDeleted": false,
			"id": "MYlA5SPL",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2161.022506471664,
			"y": 173.1037696400549,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 1152.421875,
			"height": 165.6,
			"seed": 1811767069,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "1. Ambassador API Gateway Processing:\nThe Ambassador API Gateway receives the request and processes it. \nThis processing may include tasks like routing to specific microservices, \nauthentication, and applying routing policies.",
			"rawText": "1. Ambassador API Gateway Processing:\nThe Ambassador API Gateway receives the request and processes it. \nThis processing may include tasks like routing to specific microservices, \nauthentication, and applying routing policies.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1. Ambassador API Gateway Processing:\nThe Ambassador API Gateway receives the request and processes it. \nThis processing may include tasks like routing to specific microservices, \nauthentication, and applying routing policies.",
			"lineHeight": 1.15,
			"baseline": 157
		},
		{
			"type": "text",
			"version": 282,
			"versionNonce": 471271251,
			"isDeleted": false,
			"id": "Q0nNSnSl",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2160.317753867498,
			"y": 590.8434953887531,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 1092.498046875,
			"height": 165.6,
			"seed": 1684106547,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "3. Microservice Access: \nDepending on the configuration and routing rules in the \nAmbassador API Gateway, the request may be further routed \nto one or more internal microservices within your Kubernetes cluster.",
			"rawText": "3. Microservice Access: \nDepending on the configuration and routing rules in the \nAmbassador API Gateway, the request may be further routed \nto one or more internal microservices within your Kubernetes cluster.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3. Microservice Access: \nDepending on the configuration and routing rules in the \nAmbassador API Gateway, the request may be further routed \nto one or more internal microservices within your Kubernetes cluster.",
			"lineHeight": 1.15,
			"baseline": 157
		},
		{
			"type": "text",
			"version": 268,
			"versionNonce": 440273757,
			"isDeleted": false,
			"id": "SBoK0dve",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2158.292607383124,
			"y": 411.63263926896116,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 1098.45703125,
			"height": 124.19999999999999,
			"seed": 513635197,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "2. Security and Policy Enforcement: \nThe Ambassador API Gateway enforces security and policy rules, \nsuch as access control and rate limiting, to protect the microservices.",
			"rawText": "2. Security and Policy Enforcement: \nThe Ambassador API Gateway enforces security and policy rules, \nsuch as access control and rate limiting, to protect the microservices.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2. Security and Policy Enforcement: \nThe Ambassador API Gateway enforces security and policy rules, \nsuch as access control and rate limiting, to protect the microservices.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 313,
			"versionNonce": 956343539,
			"isDeleted": false,
			"id": "TuZXv707",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3419.617477174792,
			"y": 200.53010020646093,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 1024.541015625,
			"height": 124.19999999999999,
			"seed": 985878227,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "4. Microservice Execution: \nThe request reaches the appropriate microservice within your \nKubernetes cluster, and the microservice processes the request.",
			"rawText": "4. Microservice Execution: \nThe request reaches the appropriate microservice within your \nKubernetes cluster, and the microservice processes the request.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "4. Microservice Execution: \nThe request reaches the appropriate microservice within your \nKubernetes cluster, and the microservice processes the request.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 316,
			"versionNonce": 1350473661,
			"isDeleted": false,
			"id": "qY5gJ7In",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3421.017216758126,
			"y": 406.09056570125244,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 1079.912109375,
			"height": 124.19999999999999,
			"seed": 1090255837,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "5. Response Generation: \nThe microservice processes the request and generates a \nresponse, which is then sent back to the Ambassador API Gateway.",
			"rawText": "5. Response Generation: \nThe microservice processes the request and generates a \nresponse, which is then sent back to the Ambassador API Gateway.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "5. Response Generation: \nThe microservice processes the request and generates a \nresponse, which is then sent back to the Ambassador API Gateway.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 283,
			"versionNonce": 1847955091,
			"isDeleted": false,
			"id": "Qw1Z7msL",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3412.660690065417,
			"y": 607.3256731231274,
			"strokeColor": "#000000",
			"backgroundColor": "#12b886",
			"width": 954.544921875,
			"height": 124.19999999999999,
			"seed": 1505229939,
			"groupIds": [
				"qrGemwrFquv6E25063T9E"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698277622693,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "6. Response Back to User: \nThe Ambassador API Gateway ensures that the response\nis properly routed back to the user who initiated the request.",
			"rawText": "6. Response Back to User: \nThe Ambassador API Gateway ensures that the response\nis properly routed back to the user who initiated the request.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "6. Response Back to User: \nThe Ambassador API Gateway ensures that the response\nis properly routed back to the user who initiated the request.",
			"lineHeight": 1.15,
			"baseline": 115
		},
		{
			"type": "text",
			"version": 948,
			"versionNonce": 55719518,
			"isDeleted": false,
			"id": "0E0F5ZMW",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4178.355182901564,
			"y": -1241.7776408371328,
			"strokeColor": "#000000",
			"backgroundColor": "#7950f2",
			"width": 430.8672180175781,
			"height": 84.90891828898043,
			"seed": 2054933826,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1699094060982,
			"link": null,
			"locked": false,
			"fontSize": 73.83384199041777,
			"fontFamily": 2,
			"text": "API Gateway",
			"rawText": "API Gateway",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "API Gateway",
			"lineHeight": 1.15,
			"baseline": 68
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#000000",
		"currentItemBackgroundColor": "#a089e6",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 2,
		"currentItemStrokeStyle": "dashed",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 2,
		"currentItemFontSize": 36,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 2765.6660980229126,
		"scrollY": 3561.735087617122,
		"zoom": {
			"value": 0.15000000000000002
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"colorPalette": {},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		}
	},
	"files": {}
}
```
%%