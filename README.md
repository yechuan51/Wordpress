# Wordpress
Configs I use to bring up my wordpress instance, with an Nginx reverse proxy running HTTPS.

Ideally, the whole process can be as simple as just running docker-compose a couple times. But since the server uses HTTPS and manual steps are required with certbot, this is impossible without a little effort. 

# Note
The code in this repo is unable to work by just running docker-compose. Specifically, because of the existence of the Nginx config:
https://github.com/yechuan51/Wordpress/blob/main/nginx/nginx/conf.d/default.conf

This file is meant to be copied over onto the host volume mount location. 

# End result:
https://yechuan51.com
