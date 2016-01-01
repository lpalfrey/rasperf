# RasPerf

In a nutshell
--------------

RasPerf is a fork (ish) of Raspbian which is optimised for my requirements. It was built for the RPi2

- Reduced footprint
- Reduced memory usage
- Optimised firmware settings
- Kernel optimizations
- Generally performance optimized.

After installation it should use around 400MB of disk space and 21MB of RAM. 

Note that this was build for my requirements. I am sharing it just in case anyone else finds it useful. 


Why
---

I was building a cluster which requires Wheezy (Don't ask!) and there was no minimal build of of Raspbian-Wheezy. Also, my cluster required every MB of memory I could find - so I went about reducing the memory as much as I could without breaking the Raspbian distribution (i.e, no custom kernel etc). 

There have also been some specific improvements which will help the performance of Java based applications. Although note that Java is not installed 


How
---

The default IP address is 192.168.0.51 - Either login at the console or login via SSH and change your password.

The default username and password is root/Password123

Change your hostname - /etc/hostname
Change your IP address as required - /etc/network/interfaces (note: No DHCP)
Change your DNS settings - /etc/resolve.conf (note: Resolvconf has been removed so you must put your settings in here manually)
Change host file - /etc/hosts

