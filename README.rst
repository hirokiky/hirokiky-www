hirokiky-www
============

A Web site of hirokiky.

Installation
------------

::

    pip install -r requirements.txt

Building
--------

::

    make html

Distributing
------------

Example for nginx::

    server {
        listen 80;
        server_name example.com;

        access_log /path/to/access.log;
        error_log /path/to/error.log;

        location / {
            root   /path/to/hirokiky-www/build/html/;
            index  index.html;
        }
    }
