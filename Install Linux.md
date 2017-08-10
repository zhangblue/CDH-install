# 安装Linux Red Head 6.5 64位
## 单台服务器硬件参数
> * 服务器型号：戴尔720R
> * 内存：16G
> * CPU：24核心
> * 硬盘：4T

## 服务器数量配置
> * cmserver：1台。用于运行Cloudera-Manager
> * namenode：1台。用于运行namenode
> * secondaryNamenode：1台。用于运行secondarynamenode。
> * datanode：4台。用于运行datnaode。
> 
> |服务器名称|服务器地址|
> |----------------|---------------|
> |cmserver|192.168.10.10|
> |namenode|192.168.10.11|
> |secondaryNamenode|192.168.10.22|
> |datanode01|192.168.10.12|
> |datanode02|192.168.10.13|
> |datanode03|192.168.10.14|
> |datanode04|192.168.10.15|

## 安装系统(所有服务器步骤相同)
![step1][1]

这里选择了简体中文
![step2][2]
![step3][3]
![step4][4]

设置主机名，这里使用cmserver为例。
![step5][5]

设置时区，当选了简体中文时，系统默认为`亚洲/上海`
![step6][6]

设置服务器root用户的口令
![step7][7]

对服务器硬盘进行分区。这里使用了默认分区模式，如果有需要请自行选择`创建自定义布局`选项进行手动分区。
![step8][8]

设置安装模式。这里选择`Basic Server`模式，并且自定义软件安装包。
![step9][9]

去掉`Java平台`安装包。因为系统默认为OpenJKD，而我们需要的是OracleJDK。
![step10][10]

等待安装完成。
![step11][11]
![step12][12]

## 配置IP地址
使用cmserver为例。  
编辑文件`/etc/sysconfig/network-scripts/ifcfg-em1`   
![ip][13]

## 配置HostName
使用cmserver为例。   
编辑文件`/etc/sysconfig/network`   
![hostname][13]


## 关闭iptables
关闭防火墙：`service iptables stop`   
设置防火墙开机不启动：`chkconfig iptables off`   

## 设置hosts文件
编辑文件`/etc/hosts`   
![hosts][16]

## 设置selinux文件
编辑文件`/etc/selinux/config`,将`SELINUX`的值改为`disabled`。此文件生效必须要重启系统。   
![selinux][18]


[1]:./images/system_step1.JPG
[2]:./images/system_step2.JPG
[3]:./images/system_step3.JPG
[4]:./images/system_step4.JPG
[5]:./images/system_step5.JPG
[6]:./images/system_step6.JPG
[7]:./images/system_step7.JPG
[8]:./images/system_step8.JPG
[9]:./images/system_step9.JPG
[10]:./images/system_step10.JPG
[11]:./images/system_step11.JPG
[12]:./images/system_step12.JPG
[13]:./images/system_ip.png
[16]:./images/hosts.png
[17]:./images/system_hostname.png
[18]:./images/selinux-install.png

