MongoDB 2.6 ``.deb`` 安装包自带的 ``/etc/mongodb.conf`` 配置文件里的 :setting:`~net.bind_ip`` 设置默认为
``127.0.0.1``。 在你部署 ``副本集`` 之前请注意修改这个设置，否则从别的机器上讲无法访问这个MongoDB。
