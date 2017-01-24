x264_image_transport
====================

This software is derived from the ROS packages made available by IntRoLab, Universite De Sherbrooke, Quebec, Canada.

Specifically, it provides a catkinized image transport plugin for recent versions of ROS, using x264 encoding.

Installation
============
Under current releases of Ubuntu, system installed ffmpeg libraries are too old to support this software. To get around this, do the following (tested under ROS Indigo and Ubuntu 14.04 Trusty):

Quoting from this page: http://infoheap.com/install-ffmpeg-on-ubuntu-linux/

--------------

Ubuntu Linux (14.04) does not have ffmpeg in default package source repositories. ffmpeg can be installed using mc3man ppa (personal package archive) using the following steps.

1. Add mc3man ppa to apt source

$ sudo add-apt-repository ppa:mc3man/trusty-media

2. Resynchronize the package index files from their sources

$ sudo apt-get update

3. Check where will ffmpeg be installed

$ apt-cache policy ffmpeg

ffmpeg:
  Installed: (none)
  Candidate: 7:2.8.4+git1~trusty
  Version table:
     7:2.8.4+git1~trusty 0
        500 http://ppa.launchpad.net/mc3man/trusty-media/ubuntu/ trusty/main amd64 Packages

4. Install ffmpeg using apt-get

$ sudo apt-get install ffmpeg

--------------

5. build the project using catkin_make

6. test by running: roslaunch x264_image_transport test_x264.launch

Contributors
============
Alexander Botev

Luke Teacy

License
=======
Copyright © 2014 University of Southampton. All Rights Reserved.

Redistribution and use of this software in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. The name of the author may not be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY LUKE TEACY "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
