Quick Start
===========

This document provides a guide for running a sample `SendBird` project.  
Through this project, you will be able to connect to a lobby channel, view the list of channels, and send messages to the channel.

## Running Web Sample 
You will need a local server to run the sample project. In this example, we'll be using `Python` to run our local server. 

1. Download and install Python if you don't have it.
2. Clone the project
``` bash
$ git clone https://github.com/smilefam/SendBird-JavaScript
```
3. Open terminal and run SimpleHTTPServer in project path.
``` python
$ cd basic-sample
$ python -m SimpleHTTPServer 8000
```
4. Try to connect to http://localhost:8000 in a web browser to see the sample project.

## Running React Native Sample 

1. Download and install `node` and `npm`.
2. Clone the project
``` bash
$ git clone https://github.com/smilefam/SendBird-JavaScript
```
3. Open terminal and run the following commands in the project path.
``` bash
$ cd basic-react-native-sample/SendBirdReactNativeSample
$ npm install
$ npm install -g react-native-cli
```
4. Run the sample app in iOS Simulator
``` bash
$ react-native run-ios
```

You can check out the following features when the above sample projects are running:
  1. **Open Chat List**: Connect to the sample channel, then send and receive messages.
  2. **Start Messaging**: See the list of members who've connected to the lobby channel and start a 1-on-1 or a group messaging.
  3. **Messaging List**: See or edit my list of channels.


## Integrating SendBird with an existing app

### Download the Latest SendBird JavaScript SDK
<a class="sendbird-btn sendbird-btn--green" href="https://github.com/smilefam/SendBird-SDK-JavaScript" target="_blank">Latest SendBird JavaScript SDK - Click here to download</a>  
or  
```unix
   bower install sendbird
```
or  
```unix
   npm install sendbird
```

### Add the SDK File to Your Project
After downloading the `SendBird JavaScript SDK` JavaScript file, add it to your Project Classpath (`generally the libs directory`). 

Then include the JaveScript file on your page:
```javascript
<script src="lib/SendBird.min.js"></script>
```


## Browser Compatibility
We recommend the lastest version of Chrome/Safari/Firefox/IE 10+ ( If you use older IE, please upgrade it to IE10.)




