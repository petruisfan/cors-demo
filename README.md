# Cors demo
Minimal example of using CORS.

Instructions for setting up demo using nginx:
- copy files from nginx.conf in /etc/nginx/conf.d/ . Be carefull to modify _root_ to clone location of repository.
- add records in /etc/hosts for redirecting _cors-client.com_ and _cors-server.com_ to nginx ip.
- install npm dependencies and run server:
``` bash
$> cd server
$> npm install
$> node server.js
```
- open _http://cors-client.com_ in browser.

The only catch is the response from the server must contain "Access-Control-Allow-Origin: http://cors-client.com" header.
