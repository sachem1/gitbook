### 安装 docker {#安装-docker}

1.安装必要的一些系统工具

> yum install -y yum-utils device-mapper-persistent-data lvm2

2.添加软件源信息

> yum-config-manager --add-repo[http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo](http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo)

3.更新并安装 Docker-CE

> yum makecache fast

> yum -y install docker-ce

4.设置开机Docker服务

> chkconfig docker on

5.启动docker

> service docker start

> docker version

如果 client 和server 信息都出来了,表示成功了

