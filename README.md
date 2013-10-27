a2mksite (and a2rmsite)
=======================

A quick couple of scripts that are meant to be used in conjunction with a2ensite and a2dissite that comes with apache2.

Important
---------
These scripts:

- edit your `hosts` file. *But they attempt to do so in a clean way.*
- expect that your apache configuration includes a `sites-available` and `sites-enabled` set of folders.
- are generally useless unless combined with the `a2ensite` and `a2dissite` scripts.
- are written in python rather than bash (the common convention) due to file manipulation

Installation
-------
```
cd /usr/share
git clone https://github.com/andyhu/a2mksite.git
```

Usage
-------
a2ensite:
```
a2mksite site-name.dev /site/dir
a2ensite site-name.dev.conf
/etc/init.d/apache2 reload
```
a2rmsite:
```
a2rmsite site-name.dev
```
