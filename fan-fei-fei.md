### 部署Nginx {#部署nginx}

> 1.安装依赖

```
1
 SSL
功能需要
openssl
库，直接通过
yum
安装
: yum 
install
 openssl


2
 gzip
模块需要
zlib
库，直接通过
yum
安装
: yum 
install
 zlib


3
 rewrite
模块需要
pcre
库，直接通过
yum
安装
: yum 
install
 pcre


```

> 2.使用yum安装nginx需要包括Nginx的库，安装Nginx的库

> rpm -Uvh[http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm](http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm)

> 3.安装nginx

> yum install nginx

> 4.开机启动并启动Nginx

```
1
.systemcel
 enable nginx
.service
2
.service
 nginx start


```

### docker install {#docker-install}

1. docker pull nginx

### 常见操作 {#常见操作}

1. 查看Nginx 运行的

> ps -ef \| grep nginx

2.验证配置是否正确:

> nginx -t

3.查看Nginx的版本号

> nginx -V

4.启动Nginx

> start nginx 或 systemctl start nginx

5.快速停止或关闭Nginx

> nginx -s stop

6.正常停止或关闭Nginx

> nginx -s quit

7.配置文件修改重装载命令

> nginx -s reload

8.查看nginx 配置文件是否正确

> nginx -t

### nginx 配置调整 {#nginx-配置调整}

> 1.修改运行cpu 保证以计算机的型号运行



