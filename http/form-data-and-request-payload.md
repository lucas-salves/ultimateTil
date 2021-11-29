# Form data and Request payload definitions

Request Payload is the payload body of a POST or PUT HTTP request. That is the data normally sended in POST or PUT requests.

A request with *Content-Type: application/json* look like the following:

```
POST /some-path HTTP/1.1
Content-Type: application-json

{"foo": "bar", "name": "Lucas"}
```

If you submit a HTML form with POST method and Content-Type: application/x-www-formurlencoded or Content-Type: multipart/form-data your request may look like this:

```
POST /SOME-PATH HTTP/1.1
Content-Type: application-x-www-form-urlencoded

foo=bar&name=Lucas
```

In this case the form-data is the request payload.
