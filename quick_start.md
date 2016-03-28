Quick Start
===========

This document provides a guide for running a sample `SendBird` project.  
Through this project, you will be able to connect to a lobby channel, view the list of channels, and send messages to the channel.

## Running Web Sample Project
You will need a local server to run the sample project. In this example, we'll be using `Python` to run our local server. 

1. Download and install Python if you don't have it.
  - [Download and install Python from the python website](https://www.python.org/downloads/)
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


By running the sample project, you can experience Open Chat or 1-on-1 Messaging.

- Sample project comes with a `** SendBird Sample App ID **`
- To use in a production environment ** you need to change this to your `SendBird APP ID` found on your dashboard. **

- You can check out the following features when the sample project is running:
  1. **Open Chat List**: Connect to the sample channel, then send and receive messages.
  2. **Start Messaging**: See the list of members who've connnected to the lobby channel and start a 1-on-1 or a group messaging.
  3. **Messaging List**: See or edit my list of channels.
