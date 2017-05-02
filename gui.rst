图形界面
================

第一步: 安装 X Server
------------------------------

想要在 WSL 里运行带图形界面的应用程序的话, 你首先需要在你的 Windows 电脑上安装一个 X Server. 
我推荐使用 `Xming <https://sourceforge.net/projects/xming/>`_. 

第二步: 设置 DISPLAY 环境变量
----------------------------------------

然后， 你需要通过 ``DISPLAY`` 这个环境变量来告诉你的 WSL 环境来时用你安装的 X Server。

在 ``~/.bashrc`` 里添加如下内容即可::

    export DISPLAY=:0


