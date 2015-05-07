# web2py + nginx + uwsgi installer for WebFaction

[Click here to install][1]

Web2py install/uninstall script for WebFaction using the latest stable source
code from http://www.web2py.com/examples/static/web2py_src.zip.

This installs web2py for Python 2.7, served via Nginx 1.8.0 and uWSGI 2.0.10.

The web2py files are found in ~/webapps/app_name/web2py.

IMPORTANT: Remember to set the Admin password in the extra_info field.

Caveats
-------

* Web2py won't work properly if it is mounted to a sub-URL like
http://domain.com/web2py/. Instead, it must be mounted to the website root,
e.g. http://domain.com/

* For the administrative interface to work, the web2py app must be mounted to and
accessed through an HTTPS-enabled site. You would usually mount the app to two
websites - HTTPS-disabled one for normal access, and HTTPS-enabled one for admin
logins.

  [1]:https://my.webfaction.com/new-application?script_url=https://raw.github.com/wsfulmer/webfaction-web2py-nginx-uwsgi-installer/master/install.py
