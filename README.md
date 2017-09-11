# Node-RED Samples for IBM Watson IoT Hackathon

This project contains some [Node-RED](https://nodered.org/) sample flows used in an one hour webinar to prepare attendees for an Watson IoT hackathon.

Functionality:

* Getting started with the Watson IoT Quickstart ([dashboard](https://quickstart.internetofthings.ibmcloud.com/#/)) / ([sensor](https://quickstart.internetofthings.ibmcloud.com/iotsensor/))
* Using the [IoT Starter](https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter)
* Registering IoT devices
* Building simple web user interfaces via the [Node-RED Dashboard](https://github.com/node-red/node-red-dashboard)
* Invoking REST APIs and implementing REST APIs
* Leveraging Watson services (Conversation, Translation, Tone Analyzer, Text to Speech)

![Node-RED Samples for IBM Watson IoT](https://github.com/nheidloff/node-red-watson-iot-samples/raw/master/screenshots/watson.png "Node-RED Samples for IBM Watson IoT")

Setup:

* Create a new [IoT Starter](https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter)
* Open the Node-RED editor and import [flows.json](https://github.com/nheidloff/node-red-watson-iot-samples/blob/master/flows.json)
* Add [Speech to Text](https://console.bluemix.net/catalog/services/speech-to-text?region=ibm:yp:us-south)
* Add [Language Translator](https://console.bluemix.net/catalog/services/language-translator?region=ibm:yp:us-south)
* Add [Tone Analyzer](https://console.bluemix.net/catalog/services/tone-analyzer?region=ibm:yp:us-south)
* Add [Watson Conversation](https://console.bluemix.net/catalog/services/conversation?region=ibm:yp:eu-gb). Open the Conversation tool and copy the workspace ID. Paste the ID in the Conversation node in the Node-RED flow
* Open the [device simulator](https://quickstart.internetofthings.ibmcloud.com/iotsensor/), copy the ID in the upper right corner and paste it in the IoT node on the 'IoT Quickstart' page
* Add your Twitter credentials to the two Twitter nodes
* To listen to tweets connect the Twitter node with the translator node
* Deploy the flows by pressing the red button