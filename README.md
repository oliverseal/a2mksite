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

Windows
-------

There is a very minimal support for Windows in this script. I've built them with the intention of 
creating `a2ensite` and `a2dissite` python scripts to run in windows and be used in tandem with 
something like XAMPP. That has not been done yet.
 
