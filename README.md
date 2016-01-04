# RasPerf

In a nutshell
--------------

RasPerf is a fork (ish) of Raspbian which is optimised for my requirements. It was built for the RPi2

- Reduced footprint
- Reduced memory usage
- Optimised firmware settings
- Kernel optimizations
- Generally performance optimized for the RPi2

After installation it should use around 232MB, 18MB of RAM and boot in less than 7 seconds. 

Note that this was built for my requirements. I am sharing it just in case anyone else finds it useful. 


Why
---

I needed a Rasbian version of LInux for my cluster but I required every MB of memory I could find - so I went about reducing the memory as much as I could without breaking the Raspbian distribution (i.e, no custom kernel etc). 

There have also been some specific improvements which will help the performance of Java based applications. Although note that Java is not installed 


How
---

The default IP address is 192.168.0.51 & the default username and password is root/Password123

When you login for the first time the configuration script will run which sets all of the network settings. You can run this anytime by executing /usr/bin/rasperf-setup 
