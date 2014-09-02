MongoDB安装包
-------------

MongoDB提供官方的MongoDB软件仓库(repository)供Linux的软件管理工具使用。以下是
MongoDB提供的安装包： 

- ``mongodb-org``

  这个是个超级安装包，包括下述所有的子模块。

- ``mongodb-org-server``

  这个包括MongoDB的核心数据库程序 :program:`mongod` 以及相关的配置文件和启动脚本。

- ``mongodb-org-mongos``

  这个是分片集群中用到的路由器 :program:`mongos` 程序.

- ``mongodb-org-shell``

  这个是MongoDB的命令行客户端 :program:`mongo` shell.

- ``mongodb-org-tools``

  这个包含下列MongoDB的工具: :program:`mongoimport`, 
  :program:`bsondump`, :program:`mongodump`, :program:`mongoexport`,
  :program:`mongofiles`, :program:`mongoimport`, :program:`mongooplog`,
  :program:`mongoperf`, :program:`mongorestore`, :program:`mongostat`,
  :program:`mongotop`。

控制脚本
---------------

``mongodb-org`` 安装包里有许多 :term:`控制脚本
<control script>`, 如启动脚本 |init-script-path| 等。

这个安装包的配置文件是 ``/etc/mongod.conf`` 。 关于配置文件详情请参见
:doc:`/reference/configuration-options` 。

目前为止（版本 |release| ）尚没有官方的 :program:`mongos` 的控制脚本。 
 :program:`mongos` 路由器进程仅需在 :doc:`sharding </core/sharding>` 的情景下使用。
 你可以参考 ``mongod`` 的启动脚本来写一个你自己的 :program:`mongos` 启动脚本。

