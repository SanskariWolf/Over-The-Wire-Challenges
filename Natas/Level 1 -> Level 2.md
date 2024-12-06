Challenge Information

Natas Level 1 → Level 2

Username: natas2
URL:      http://natas2.natas.labs.overthewire.org


Solution

1. Got for the source code. 

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
<script>var wechallinfo = { "level": "natas2", "pass": "TguMNxKo1DSa1tujBLuZJnDUlCcUAPlI" };</script></head>
<body>
<h1>natas2</h1>
<div id="content">
There is nothing on this page
<img src="files/pixel.png">
</div>
</body></html>

```

2. The line src="files/pixel.png" is a different one. Basically website is also kind of directory. Just like how we nacigate through directories in a normal system. For a website routing is performed in a similar manner. 

3. Go for /files page by http://natas2.natas.labs.overthewire.org/files


Index of /files
[ICO]	Name	Last modified	Size	Description
[PARENTDIR]	Parent Directory	 	- 	 
[IMG]	pixel.png	2024-09-19 07:03 	303 	 
[TXT]	users.txt	2024-09-19 07:03 	145 	 
Apache/2.4.58 (Ubuntu) Server at natas2.natas.labs.overthewire.org Port 80


4. Check users.txt file

# username:password
alice:BYNdCesZqW
bob:jw2ueICLvT
charlie:G5vCxkVV3m
natas3:3gqisGdR0pjm6tpkDKdIWO2hSvchLeYH
eve:zo4mJWyNj2
mallory:9urtcpzBmH

5. Here we have the password 3gqisGdR0pjm6tpkDKdIWO2hSvchLeYH
