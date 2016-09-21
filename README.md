Welcome to Nsu Lead Service!
----------------------------


Nsu lead services is an webservice that is provider for Private Florida Research University | Nova Southeastern University. To send leads in our system

Current version:  v0.0.1

http://fldvd-apinet01.ad.nova.edu/appcentral/lms/instances/-1/forms/PostExternalRequestVendor


Get started
-------------

First of all you need an api key, you can get youe own key on vendor section:

<img src="../assets/images/vendor-key.PNG" width="200">

> **Note:**

> - This key must be saved properly.
> - If you send multiple times the same info the system is going to reject the repeated data.

Test endpoint
------

To do:


 Set your header key

<img src="../assets/images/Header.PNG" width="200">
 
  Create a body with the request (See in this documentation the option available fields)
 
<img src="../assets/images/fields.PNG" width="200">

You can test our endpoint using postman we prepare an example in this link:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/3dae32e8817304601d97)


 

Languajes suport examples
-------------------------

Javascript
----------

.

Ajax
----

Implementation on javascript code

```js

var settings = {
  "async": true,
  "crossDomain": true,
  "url": <URL>,
  "method": "POST",
  "headers": {
    "key_vendor": "YOURKEY",
    "content-type": "application/json",
  },
  "processData": false,
  "data": "DATA"
}

$.ajax(settings).done(function (response) {
  console.log(response);
});

```

C Sharp
----

Implementation on javascript c#

```js
var client = new RestClient(<URL>);
var request = new RestRequest(Method.POST);
request.AddHeader("cache-control", "no-cache");
request.AddHeader("content-type", "application/json");
request.AddHeader("key_vendor", <KEY>);
request.AddParameter("application/json", <JSON-STRINGIFY>, ParameterType.RequestBody);
IRestResponse response = client.Execute(request);

```

JAVA
----

Implementation on java code

```js
HttpResponse<String> response = Unirest.post(<URL>)
  .header("key_vendor", <Key>)
  .header("content-type", "application/json")
  .header("cache-control", "no-cache")
  .body(<JSON-STRINGIFY>)
  .asString();

```

NODE
----

Implementation on node code

```js
var request = require("request");

var options = { method: 'POST',
  url: <URL>,
  headers: 
   { 
     'cache-control': 'no-cache',
     'content-type': 'application/json',
     key_vendor: <KEY> },
  body: 
   <JSON-OBJECT>,
  json: true };

request(options, function (error, response, body) {
  if (error) throw new Error(error);

  console.log(body);
});


```

PHP
----

Implementation on php code

```js
<?php

$request = new HttpRequest();
$request->setUrl(<URL>);
$request->setMethod(HTTP_METH_POST);

$request->setHeaders(array(
  'cache-control' => 'no-cache',
  'content-type' => 'application/json',
  'key_vendor' => <YOURKEYHERE>
));

$request->setBody(<JSON-OBJECT>);

try {
  $response = $request->send();

  echo $response->getBody();
} catch (HttpException $ex) {
  echo $ex;
}


```
