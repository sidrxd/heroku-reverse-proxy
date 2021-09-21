# Reverse Proxy on Heroku

Run a reverse proxy using nginx on Heroku.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Installation

Use the [Deploy to Heroku](https://heroku.com/deploy) button above to create a
copy of the app, then Set `UPSTREAM_SERVER`, `PASSWORD`, `USERNAME` config vars.

eg.

_UPSTREAM_SERVER = https://www.google.com_

_PASSWORD = password_

_USERNAME =  username_

## What's New

- Basic Authentication. With a [.profile.d](https://devcenter.heroku.com/articles/buildpack-api#profile-d-scripts) script, it is possible to generate an `.htpasswd` file on dyno boot that contains a username and password in config vars. This file can then be used by nginx for basic authentication. 

- Anti Spider strategy  


## Credits

- Updated to heroku-20 stack and recent community build pack for nginx.
- Based on [funwhilelost/heroku-reverse-proxy](https://github.com/funwhilelost/heroku-reverse-proxy),
- Based on [octoberswimmer/heroku-reverse-proxy](https://github.com/octoberswimmer/heroku-reverse-proxy),
- originally forked from [api-proxy-3scale-heroku](https://github.com/Taytay/api-proxy-3scale-heroku).

## Reference
- [Heroku上のPHPアプリケーションにBASIC認証を導入する](https://mistymagich.wordpress.com/2016/02/12/nginx-basic-authentication-in-php-on-heroku/)
