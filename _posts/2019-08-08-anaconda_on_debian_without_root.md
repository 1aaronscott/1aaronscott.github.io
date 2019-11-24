---
layout: post
title: Installing Anaconda on Debian Without Root
subtitle: LS assignment
tags: [blog]
comments: true
---
Here are the steps I've taken to get the Anaconda distribution installed on Debian. Anaconda describes itself as an "open-source [d]istribution" which "is the easiest way to perform Python/R data science and machine learning on Linux." It packages other projects such as pandas, matplotlib, and jupyter notebooks along with its own conda application. Searching for instructions on google will lead to several pages stating root privileges are necessary which is not only untrue but ill-advised.

1. Go to the [Anaconda downloads page](https://www.anaconda.com/download/#linux) and select the appropriate file. Anaconda doesn't have a url that always points to the latest version so you'll have to choose manually. 

2. Download the shell script with wget or curl [INSERT EXAMPLES] and do an integrity check with md5sum [INSERT SAMPLE COMMAND]. Anaconda has a page for [hashes of all their files](https://docs.anaconda.com/anaconda/install/hashes/lin-3-64/). 

3. Execute "bash [Anaconda filename" and it will ask you to accept the license (BSD) default to installing all packages to $HOME/anaconda3 (or similar). The install took less than a minute for me and used about 3.3 gigabytes of drive space.


