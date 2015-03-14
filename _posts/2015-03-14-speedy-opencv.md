---
layout: post
title: speedy OpenCV
categories: opencv computer vision
tags: []
published: True

---

A new OpenCV install is often source of headache. For the beta version of 3.0 I found this procedure particularly easy (on Mac OSX 10.10):

 - `cd ~/<my_working_directory>`
 - `git clone https://github.com/Itseez/opencv.git`
 
 Once downloaded:

 - `cd ~/<my_working_directory>/opencv`
 - `mkdir build`
 - `cd build`

 Configuring:

 - `cmake -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX=/usr/local ..`

 Build:

 - `make`

 Install from build directory:

 - `sudo make install`

 That's it!

