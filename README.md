# php-proxy-app
Web Proxy Application built on [**php-proxy library**](https://github.com/Athlon1600/php-proxy) ready to be installed on your server

![alt text](http://i.imgur.com/KrtU5KE.png?1 "This is how PHP-Proxy looks when installed")

## Installation

Keep in mind that this is a **project** and not a library. Installing this via *require* would do you not good.
A project such as this, should be installed straight into the public directory of your web server.

```bash
composer create-project shirtjs/titanium-new:dev-master /var/www/
```

If you do not have composer or trying to host this application on a **shared hosting**, then download a pre-installed version of this app as a ZIP archive from [**www.radioactivehalflife.cf/download.html**](https://www.radioactivehalflife.cf/download.html).


## Keep it up-to-date

Application itself rarely will change, vast majority of changes will be done to its requirement packages like php-proxy, and OpenNews. Simply call this command once in a while to make sure your proxy is always using the latest versions.

```
composer update
```

#### config.php

This file will be loaded into the global Config class. Changing this will allow you to set encoding options, URL options, etc.

#### /templates/

This should have been named "views", but for historic purposes we keep it named as templates for now. Change these files if you want your proxy to look cosmetically different.

#### /plugins/

PHP-Proxy provides many of its own native plugins, but users are free to write their own custom plugins, which could then be automatically loaded from this very folder. See /plugins/TestPlugin.php for an example.

#### /css/

Edit the appearance and functionality of your "news site".

#### /images/

Add/remove/edit images that show on the "news site".

#### /js/

Change the scripts that make your "news site" work.

#### /screenshots/

Folder serves no purpose to anyone; it's just here.
