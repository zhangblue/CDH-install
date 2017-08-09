# 搭建yum源
## 在所有服务器中进行相同操作
> * 进入`/etc/yum.repos.d/`目录
> * 将`CentOS-Base.repo`文件重命名为`CentOS-Base.repo.bak`
> * 执行命令`curl -O http://192.168.10.10/cm5/redhat/6/x86_64/cm/cloudera-manager.repo`。这时目录中会出现名为`cloudera-manager.repo`的文件
 ![yum-deploy1][1]
> * 执行命令`yum clean all`清空yum源列表
> * 执行命令`yum list`刷新yum源列表，这时会出现以下内容
> ![yum-deploy1][2]

[1]:./images/yum-deploy1.png
[2]:./images/yum-list.png