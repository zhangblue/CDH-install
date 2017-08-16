# CDH默认数据库
## 说明
> * 在采用Cloudera-Manager安装cdh时，通常使用内嵌的PostgreSQL数据库。
> * Cloudera-Manager除了保存CDH集群的配置元数据的scm数据库外，还为Activity Monitor（活动监控）、Service Monitor（服务监控）、Report Manager（报告管理）、Host Monitor（主机监控）、Cloudera Navigator（Cloudera导航）等信息分别创建数据amon、smon、rmon、hmon、nav相应的数据。
> * 如果你运行了Hive服务，Cloudera-Manager还会创建hive数据库用于保存hive metastore即建表的元数据等。

## 数据库信息

> * 使用内嵌PostgresSQL数据安装完成CDH时，在CDH管理页面会有如下说明   
> ![database_default1][1]   
> 如果要在生产环境中使用CDH，请根据链接中的官方教程进行配置。
> * scm数据库的用户名，密码   
> 文件：`/etc/cloudera-scm-server/db.properties`
> ![database_default2][2]
> 根据文件内容，可以进入到数据库中查看数据。   
> `psql -p 7432 scm scm`
> * 其他数据库(如`Activity Monitor`,`Host Monitor`,`Service Monitor`,`Report Manager`,`Cloudera Navigator`)的用户名、密码   
> 文件：`/etc/cloudera-scm-server/db.mgmt.properties`
> ![database_default3][3]
> * 数据库管理者(相当于oracle DBA)cloudera-scm的用户名、密码
> 文件：`/var/lib/cloudera-scm-server-db/data/generated_password.txt`
> ![database_default4][4]

[1]:./images/database_default1.png
[2]:./images/database_default2.png
[3]:./images/database_default3.png
[4]:./images/database_default4.png