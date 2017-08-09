# 下载CDH安装包

## 下载RPM包
地址：`http://archive.cloudera.com/cm5/redhat/6/x86_64/cm/5.11.1/`
下载此地址下的所有内容。并且在httpd服务中创建相同的目录结构，

![download-rpm][1]

httpd服务目录   
![download-rpm2][2]

## 下载验证文件
下载   
`http://archive.cloudera.com/cm5/redhat/6/x86_64/cm/RPM-GPG-KEY-cloudera`
和   
`http://archive.cloudera.com/cm5/redhat/6/x86_64/cm/cloudera-manager.repo`

![download-rpm3][3]
并且也要创建相同的目录

编辑`cloudera-manager.repo`文件，修改后的内容如下：
![download-rpm4][4]

## 下载parcels文件
下载地址：   
`http://archive.cloudera.com/cdh5/parcels/5.11.1/`

下载后要在httpd服务器中创建相同的内容
![download-rpm5][5]

## Httpd目录最终效果
![download-rpm6][6]
![download-rpm7][7]
![download-rpm8][8]
![download-rpm9][9]
![download-rpm10][10]

## 下载安装向导.bin文件
下载地址：   
`http://archive.cloudera.com/cm5/installer/5.11.1/`

此文件不需要在httpd服务器中创建相同文件，放在任意目录都可以。

![download-rpm11][11]


[1]:./images/download-rpm.png
[2]:./images/download-rpm2.png
[3]:./images/download-rpm3.png
[4]:./images/download-rpm4.png
[5]:./images/download-rpm5.png
[6]:./images/download-rpm6.png
[7]:./images/download-rpm7.png
[8]:./images/download-rpm8.png
[9]:./images/download-rpm9.png
[10]:./images/download-rpm10.png
[11]:./images/download-rpm11.png