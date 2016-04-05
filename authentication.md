# Authentication

### Login with UserId only

SendBird requires only UserId and Nickname to login in Client SDK by default.

It creates a user account on demand if UserId has not been taken yet. 

UserId could be any unique string id such as email, uid in your database.

This simple authentication is useful when you are in development or your service doesn't need additional security.

```javascript
sendbird.init({
    "app_id": appId,
    "guest_id": guestId,
    "user_name": nickName,
    "image_url": '',
    "access_token": '',
    "successFunc": function(data) {
      // Login succeede.
    },
    "errorFunc": function(status, error) {
      console.log(status, error);
    }
  });
```

### Login with UserId and AccessToken

With SendBird [Server API](https://sendbird.gitbooks.io/sendbird-server-api/content/en/user.html), you can create a user with an access token or issue an access token for an existing user. Once the access token is issued for the user, you should provide the correct access token in `init` method. 

* Create a SendBird user account via Server API when your user signs up your service.
* Save the access token to your secured persistent store.
* Load the access token in your client and pass it to SendBird `login` method.
* Issue a new access token via Server API and update it in your persistent store periodically.

```javascript
sendbird.init({
    "app_id": appId,
    "guest_id": guestId,
    "user_name": nickName,
    "image_url": '',
    "access_token": access_token,
    "successFunc": function(data) {
      // Login succeede.
    },
    "errorFunc": function(status, error) {
      console.log(status, error);
    }
  });
```
