## Overview

Yum-axelget is a plugin for yum that accelerates download rate with multi-threads by axel. 

Feature:

 - Use axel to download rpm pakcage, as well as delta package(a.k.a drpm or presto)
 - Also download repo metadata based on yum.conf.mdpolicy 
 - Format the output of axel and let it look like default yum progress bar

## Download

You can get the program from https://github.com/crook/yum-axelget/releases.

or get latest codes:

    git clone https://github.com/crook/yum-axelget

## Installation

Before install yum-axelget, you need to install the following dependences:

    sudo yum install axel
    sudo yum install yum-plugin-fastestmirror

Now 'yum-axelget' are in Fedora Official Repository. 
On Fedora, use this command to install:

    sudo yum install yum-axelget

Run 'sudo python setup.py install' in source directory.
or:

    sudo cp axelget.conf /etc/yum/pluginconf.d/
    sudo cp axelget.py  /usr/lib/yum-plugins/

## Debug

Run `sudo /usr/bin/yum --debuglevel=3 YumCommand`

Please send the console output of the above command for help and support

## Contribution

- Get code from https://github.com/crook/yum-axelget
- Change and test in your localhost
- Send pull request to https://github.com/crook/yum-axelget
- You can also help to review patches in https://github.com/crook/yum-axelget/pulls

## Help&Support

Disable axelget plugin firstly to check yum is working well:

    sudo yum --disableplugin=axelget YumCommand

If yes, it should be a bug with yum-axelget.

Please report your problem by create a new issue in github:
https://github.com/crook/yum-axelget/issues

Or send email to Ray Chen <chenrano2002@gmail.com>

