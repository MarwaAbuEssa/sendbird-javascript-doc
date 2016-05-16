# Event Handler
Define event functions that handle various events.

```javascript
sendbird.events.onMessageReceived = function(obj) {
  console.log(obj);
  // do something
};

sendbird.events.onSystemMessageReceived = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onFileMessageReceived = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onBroadcastMessageReceived = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onMessagingChannelUpdateReceived = function(obj) {
  console.log(obj);
  // do something...
};


sendbird.events.onTypeStartReceived = function(obj) {
  console.log(obj);
  // do something...
}

sendbird.events.onTypeEndReceived = function(obj) {
  console.log(obj);
  // do something...
}

sendbird.events.onReadReceived = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onMessageDelivery = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onBanReceived = function(obj) {
  console.log(obj);
  // do something...
};

sendbird.events.onReconnectFailed = function() {
  // do something...
}

```

 * **onMessageReceived**: The function is called when a generic message has been received.
 * **onSystemMessageReceived**: The function is called when a system message has been received.
 * **onFileMessageReceived**: The function is called when a file message has been received.
 * **onBroadcastMessageReceived**: The function is called when a broadcast message has been received.
 * **onMessagingChannelUpdateReceived**: The function is called when a 1-on-1 Messaging channel/Group Messaging channel has been updated.
 * **onTypeStartReceived**: The function is called when a typing start message has been received.
 * **onTypeEndReceived**: The function is called when a typing end message has been received.
 * **onReadReceived**: The function is called when signal that other user read message in messaging channel has been received.
 * **onMessageDelivery**: The function is called when a message has been sent.  
 * **onBanReceived**: The function is called when a ban message has been received.  
 * **onReconnectFailed**: The function is called when reconnect is failed.  



#### Event object
Event object passed by event functions has the following format.

```json
  {
    "data": string,        // reserved data. will come soon.
    "message": string,     // message string
    "ts": int,             // timestamp
    "user": {
      "guest_id": string,  // user unique id
      "image": string,     // user profile image url
      "name": string       // user nickname
    }
  }
```

 * **other fields**: Internal use only or deprecated 