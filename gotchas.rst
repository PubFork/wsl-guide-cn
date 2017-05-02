
常见问题解答
==============

VIM 里方向键不管用了
-------------------------

你可能会注意到, 默认情况下 WSL 里的 Vim 的方向键不工作了。要修复这个故障， 你需要在你的 ``~/.vimrc`` 里添加如下内容::

    $ cat ~/.vimrc
    set term=builtin_ansi

Sudo 时会显示 'Unable to Resolve Host' 这样的警告
-------------------------------------

You may notice that every time you run ``sudo something``, your system complains that it cannot resolve it's own hostname, but then continues on anyway. To fix this annoyance, you need to add your system's hostname to ``/etc/hosts``::

    $ cat /etc/hosts
    127.0.0.1 localhost
    127.0.0.1 nova
    ...

Here, my machine is called 'nova'. 