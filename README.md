Welcome to Nsu Lead Service!
----------------------------


Nsu lead services is an webservice that is provider for Private Florida Research University | Nova Southeastern University. To send leads in our system

Current version:  v0.0.1

http://localhost:8540/lms/instances/-1/forms/PostExternalRequestVendor


Get started
-------------

First of all you need an api key, you can get youe own key on vendor section:

<img src="https://lh5.googleusercontent.com/OMa2_kyFzUKLpr_f5v1BZRBa135RMygMu3avRrzGfvDodbAQA9WRKI4ttUbETs1Sm046d-WSAXteqKs=w1366-h599-rw" width="200">

> **Note:**

> - This key must be saved properly.
> - If you send multiple times the same info the system is going to reject the repeated data.

Languajes suport examples
-------------------------

Javascript
----------

.

Ajax

```js

var settings = {
  "async": true,
  "crossDomain": true,
  "url": 'currenturl',
  "method": "POST",
  "headers": {
    "key_vendor": "YOURKEY",
    "content-type": "application/json",
  },
  "processData": false,
  "data": "DATA"
}
```

