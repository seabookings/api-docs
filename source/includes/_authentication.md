# Authentication

> To authorize, we currently use a JWT strategy.


```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: Bearer my_own_token"
```

```javascript
// make the request to the login endpoint

function getToken() {
  var xmlHttp = new XMLHttpRequest();
  xmlHttp.open( "GET", "/api/v1/auth/anonymous/token", false ); // false for synchronous request
  xmlHttp.send( null );
  return JSON.parse(xmlHttp.responseText).token;
}

var token = getToken();
var xhr = new XMLHttpRequest();
var xhr.setRequestHeader("Authorization", "Bearer " + token);

// Then select an api endpoint and send the request

```

> Make sure to replace `my_own_token` with your JSON Web Token.

SeaBookings uses JWT to allow access to the API. You can get an anonymous token by making a request to `/api/v1/auth/anonymous/token`

SeaBookings expects for the JWT key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer my_own_token`

<aside class="notice">
You must replace <code>my_own_token</code> with your personal JWT.
</aside>