Challenge Information

Natas Level 2 → Level 3

Username: natas3
URL:      http://natas3.natas.labs.overthewire.org


Solution

1. Go straight for the source code.

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
<script>var wechallinfo = { "level": "natas3", "pass": "3gqisGdR0pjm6tpkDKdIWO2hSvchLeYH" };</script></head>
<body>
<h1>natas3</h1>
<div id="content">
There is nothing on this page
<!-- No more information leaks!! Not even Google will find it this time... -->
</div>
</body></html>
```

2. Whevever there is Google, it's either related to the topic of Search Engine Optimiation or Google Agent.{Most of the times.}
3. Check robots.txt page by http://natas3.natas.labs.overthewire.org/robots.txt

```
User-agent: *
Disallow: /s3cr3t/
```

4. You have  hidden path. Go for it. http://natas3.natas.labs.overthewire.org/s3cr3t/

```
Index of /s3cr3t
[ICO]	Name	Last modified	Size	Description
[PARENTDIR]	Parent Directory	 	- 	 
[TXT]	users.txt	2024-09-19 07:03 	40 	 
Apache/2.4.58 (Ubuntu) Server at natas3.natas.labs.overthewire.org Port 80
```

5. Check users.txt

natas4:QryZXc2e0zahULdHrtHxzyYkj59kUxLQ


6. You got the password QryZXc2e0zahULdHrtHxzyYkj59kUxLQ