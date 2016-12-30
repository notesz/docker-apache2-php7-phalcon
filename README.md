Apache2/PHP7/Phalcon3 docker image
==================================

A webserver environment docker image with Apache 2, PHP 7 (with error display) and Phalcon 3 based on Ubuntu.


Installed packages
-------------------
* Ubuntu Server 16.04
* Apache 2
* PHP 7.0
* PHP 7.0-curl
* PHP 7.0-gd
* PHP 7.0-json
* PHP 7.0-mysql
* PHP 7.0-intl
* PHP 7.0-mbstring
* PHP 7.0-mcrypt
* php-imagick
* Phalcon 3.03

Usage
------

For example:

* Hostname is: test.project
* Your project's directory is /home/notesz/webdev/testProject
* Your project's documentroot is /home/notesz/webdev/testProject/public

Usage with options:

```bash
docker run -d --hostname test.project \
    -v /home/notesz/webdev/testProject:/var/www \
    -p 80:80 \
    --name test.project \
    notesz/apache2-php7-phalcon
```

* `-p [local port]:80` local port to the container's HTTP port 80
* `--name [name]` name
