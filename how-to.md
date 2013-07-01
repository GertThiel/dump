# How to … #

* How to [flush the DNS cache](http://www.tech-faq.com/how-to-flush-dns.html)

  Mac OS X:

        dscacheutil -flushcache

  Windows:

        ipconfig /flushdns

* How to [list the installed packages](http://www.howtogeek.com/howto/linux/show-the-list-of-installed-packages-on-ubuntu-or-debian/) on Debian or Ubuntu

  Get the list of installed packages:

        dpkg --get-selections
        dpkg --get-selections | grep php

  Get a list of files installed with a package:

        dpkg -L php5-gd
