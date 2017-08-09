# 安装依赖包
## cmserver主机
挂载USB移动光驱`mount /dev/cdrom1 /mnt/`
在光盘目录`/mnt/Packages`中找到如下rmp包

使用`rpm -ivh xxxxx.rpm`命令进行安装

```
* apr-1.3.9-5.el6_2.x86_64.rpm
* apr-util-1.3.9-3.el6_0.1.x86_64.rpm
* httpd-tools-2.2.15-29.el6.centos.x86_64.rpm
* apr-util-ldap-1.3.9-3.el6_0.1.x86_64.rpm
* httpd-2.2.15-29.el6.centos.x86_64.rpm
* fuse-libs-2.8.3-4.el6.x86_64.rpm
* fuse-2.8.3-4.el6.x86_64.rpm
* mod_ssl-2.2.15-29.el6.centos.x86_64.rpm
* MySQL-python-1.2.3-0.3.c1.1.el6.x86_64.rpm
* postgresql-libs-8.4.18-1.el6_4.x86_64.rpm
* postgresql-8.4.18-1.el6_4.x86_64.rpm
* postgresql-server-8.4.18-1.el6_4.x86_64.rpm
* python-psycopg2-2.0.14-2.el6.x86_64.rpm
* pkgconfig-0.23-9.1.el6.x86_64.rpm
* libsepol-devel-2.0.41-4.el6.x86_64.rpm
* libselinux-devel-2.0.94-5.3.el6_4.1.x86_64.rpm
* libcom_err-devel-1.41.12-18.el6.x86_64.rpm
* keyutils-libs-devel-1.4-4.el6.x86_64.rpm
* krb5-devel-1.10.3-10.el6_4.6.x86_64.rpm
* zlib-devel-1.2.3-29.el6.x86_64.rpm
* openssl-devel-1.0.1e-15.el6.x86_64.rpm

```

## 其他主机
使用rpm -ivh 命令进行安装

```
* apr-1.3.9-5.el6_2.x86_64.rpm
* apr-util-1.3.9-3.el6_0.1.x86_64.rpm
* httpd-tools-2.2.15-29.el6.centos.x86_64.rpm
* apr-util-ldap-1.3.9-3.el6_0.1.x86_64.rpm
* httpd-2.2.15-29.el6.centos.x86_64.rpm
* fuse-libs-2.8.3-4.el6.x86_64.rpm* fuse-2.8.3-4.el6.x86_64.rpm
* mod_ssl-2.2.15-29.el6.centos.x86_64.rpm
* MySQL-python-1.2.3-0.3.c1.1.el6.x86_64.rpm
* postgresql-libs-8.4.18-1.el6_4.x86_64.rpm
* python-psycopg2-2.0.14-2.el6.x86_64.rpm
* pkgconfig-0.23-9.1.el6.x86_64.rpm
* libsepol-devel-2.0.41-4.el6.x86_64.rpm
* libselinux-devel-2.0.94-5.3.el6_4.1.x86_64.rpm
* libcom_err-devel-1.41.12-18.el6.x86_64.rpm
* keyutils-libs-devel-1.4-4.el6.x86_64.rpm
* krb5-devel-1.10.3-10.el6_4.6.x86_64.rpm
* zlib-devel-1.2.3-29.el6.x86_64.rpm
* openssl-devel-1.0.1e-15.el6.x86_64.rpm
```