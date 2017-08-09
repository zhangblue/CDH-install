# 配置Httpd服务
## 说明
> * 因为网络原因，使用在线安装的方式速度非常慢，所以这里使用离线的方式进行安装，但为了保证整体安装步骤不变，故需要配置一个Httpd服务来模拟在线安装。
> * 此服务只需要在某一台服务器中安装。这里我选择安装在cmserver服务器上。

## 启动Httpd服务
启动httpd服务：`service httpd start`   
手动在`/var/www/html/`目录中创建test目录，并放入一个文件来测试httpd是否运行正常

浏览器访问`http://192.168.10.10/test/`看到如下内容表示运行正常。
![check-httpd][1]

[1]:./images/httpd-check.png

