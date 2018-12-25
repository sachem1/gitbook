\#\#\# 部署Nginx



&gt; 1.安装依赖

\`\`\`

　1 SSL功能需要openssl库，直接通过yum安装: yum install openssl



　2 gzip模块需要zlib库，直接通过yum安装: yum install zlib



　3 rewrite模块需要pcre库，直接通过yum安装: yum install pcre



\`\`\`

&gt; 2.使用yum安装nginx需要包括Nginx的库，安装Nginx的库



&gt; rpm -Uvh http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm



&gt; 3.安装nginx



&gt; yum install nginx



&gt; 4.开机启动并启动Nginx

\`\`\`

1.systemcel enable nginx.service

2.service nginx start



\`\`\`



\#\#\# docker install

1. docker pull nginx 





\#\#\# 常见操作



1. 查看Nginx 运行的

&gt; ps -ef \| grep nginx 



2.验证配置是否正确:

&gt; nginx -t



3.查看Nginx的版本号

&gt; nginx -V



4.启动Nginx

&gt; start nginx 或 systemctl start nginx



5.快速停止或关闭Nginx

&gt; nginx -s stop



6.正常停止或关闭Nginx

&gt; nginx -s quit



7.配置文件修改重装载命令

&gt; nginx -s reload



8.查看nginx 配置文件是否正确

&gt; nginx -t



 

 

 

 

 

 \#\#\# nginx 配置调整

 &gt; 1.修改运行cpu 保证以计算机的型号运行

