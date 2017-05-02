更新 WSL
============

更新 WSL 里的软件包
------------------------

因为 WSL 就是一个标准的 Ubuntu 系统， 升级你的软件包(package) 就像操作普通 Ubuntu 一样::

    $ sudo apt-get update
    $ sudo apt-get upgrade

更新 Ubuntu 系统
----------------------

你也可以通过下列命令来把 Ubuntu 系统本身升级到最新版本 (注意， 这个更新会花费较长时间)!::

    $ sudo -S apt-mark hold procps strace sudo
    $ sudo -S env RELEASE_UPGRADER_NO_SCREEN=1 do-release-upgrade

就像你预料的那样, 大功告成了!
