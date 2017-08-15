# 配置ntp服务
##说明
> * 因集群中各节点需要保证时钟统一。所以需要配置一个ntp服务器来进行服务器之间的时钟同步。
> * `ntp server`端运行在cmserver上，`ntp client`端运行在其余设备上

## 配置
因为集群之间要保证时钟准确，所以需要配置NTP服务。   
使用cmserver服务器作为ntp server端，其他服务器作为ntp client端。   
服务端：编辑`/etc/ntp.conf`文件，加入内容`restrict 192.168.10.0 mask 255.255.255.0 nomodify`表示信任10段的所有服务器   
![ntp-server][14]

客户端：
添加向cmserver服务器同步时间
![ntp-client][15]

启动ntp服务:`service ntpd start`   
设置ntp服务开机自启动:`chkconfig ntpd on`

[14]:./images/ntp_server.png
[15]:./images/ntp_client.png
