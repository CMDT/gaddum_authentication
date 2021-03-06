# gaddum_authentication
a wrapper service which holds app-ids on behalf of an insecure client

Please see the following items for inspiration:

* [cordova plugin](https://github.com/Festify/cordova-spotify-oauth)
* [tutorial](https://devdactic.com/ionic-spotify-app-oauth/)


Current deployment is at:
https://gaddumauth.herokuapp.com/

Swagger UI is at:
https://gaddumauth.herokuapp.com/docs/

This application can be deployed from localhost for debugging. Make sure the client mobile app is on the same wireless local network. The urls used look like this, for example:

http://192.168.1.5:8000/spotify/exchange
http://192.168.1.5:8000/spotify/refresh


The server must define the following environment variables:


|var|example|
|-|-|
|API_DOMAIN|gaddumauth.herokuapp.com| 
|API_PORT|443|
|API_SCHEME|https|
|SPOTIFY_API_DOMAIN|accounts.spotify.com|
|SPOTIFY_API_PATH|/api/token| 
|SPOTIFY_CLIENT_CALLBACK_URL|gaddumspotify://callback| 
|SPOTIFY_CLIENT_ID| obtained from dev account|
|SPOTIFY_CLIENT_SECRET|obtained from dev account |
|SPOTIFY_ENCRYPTION_SECRET|known to server and client|
 
