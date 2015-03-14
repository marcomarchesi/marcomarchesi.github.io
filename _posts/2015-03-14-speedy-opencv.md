---
layout: post
title: speedy OpenCV
categories: opencv computer vision
tags: []
published: True

---

A new OpenCV install is often source of headache. For the beta version of 3.0 I found this procedure particularly easy (on Mac OSX 10.10):

 1) `cd ~/<my_working_directory>`
 2) `git clone https://github.com/Itseez/opencv.git`
 
 Once downloaded:

 3) `cd ~/<my_working_directory>/opencv`
 4) `mkdir build`
 5) `cd build`

 Configuring:

 6) `cmake -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX=/usr/local ..`

 Build:

 7) `make`

 Install from build directory:

 8) `sudo make install`

 That's it!

 