# 安装Cloudera Manager
## 安装
> * 对之前下载好的`cloudera-manager-install.bin`文件赋可执行权限`chmod +x cloudera-manager-install.bin`，并执行。
> * 在弹出的对话框中一直选择下一步。直到进行安装，等待安装完成。
> ![bin-install][1]
> * 安装完成后，需要等5分钟左右。使用浏览器访问地址`http://192.168.10.10:7180/，进行配置。默认用户名和密码都为admin`
> ![cdh-login][2]
> * 根据页面内容进行配置
> ![cdh-install-step2][3]
> * 选择免费版本
> ![cdh-install-step3][4]
> ![cdh-install-step4][5]
> * 输入要安装的服务器地址，点击搜索。
> ![cdh-install-step5][6]
> * 显示搜索到的服务器列表
> ![cdh-install-step6][7]
> * 选择`使用Parcel(建议)`,并且点击`更多选项`
> ![cdh-install-step7][8]
> * 删除`远程Parcel存储库URL`中的所有选项，只保留第一项，内容填写为httpd服务的url地址
> ![cdh-install-step8][9]
> * 此时会出现`选择CDH的版本 CDH-5.11.1-1.cdh5.11.1.p0.4`。下面的`自定义存储库`填写httpd中下载的url
> ![cdh-install-step9][10]
> * 勾选安装JDK
> ![cdh-install-step10][11]
> * 设置root口令
> ![cdh-install-step11][12]
> * 等待安装完成
> ![cdh-install-step12][13]
> ![cdh-install-step13][14]
> * 根据提示修正告警
> ![cdh-install-step14][15]
> * 修正完成后点击`重新运行`检查是否修正完成。
> ![cdh-install-step15][16]
> * 此处不作任何安装操作，直接关闭页面，然后重新访问页面。
> ![cdh-install-step16][17]
> * 选择`添加Cloudera Management Service`
> ![cdh-install-step17][18]
> ![cdh-install-step18][19]
> * 等待安装完成
> ![cdh-install-step19][20]
> ![cdh-install-step20][21]

[1]:./images/bin-install.png
[2]:./images/cdh-login.png
[3]:./images/cdh-install-step2.png
[4]:./images/cdh-install-step3.png
[5]:./images/cdh-install-step4.png
[6]:./images/cdh-install-step5.png
[7]:./images/cdh-install-step6.png
[8]:./images/cdh-install-step7.png
[9]:./images/cdh-install-step9.png
[10]:./images/cdh-install-step10.png
[11]:./images/cdh-install-step11.png
[12]:./images/cdh-install-step12.png
[13]:./images/cdh-install-step14.png
[14]:./images/cdh-install-step15.png
[15]:./images/cdh-install-step16.png
[16]:./images/cdh-install-step17.png
[17]:./images/cdh-install-step18.png
[18]:./images/cdh-install-step19.png
[19]:./images/cdh-install-step20.png
[20]:./images/cdh-install-step21.png
[21]:./images/cdh-install-step22.png
