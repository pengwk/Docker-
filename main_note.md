# Docker

## Docker Run

### Dockerfile 编写

## Docker Compose

### docker-compose.yml 编写


## 

## 常用软件的安装

软件的配置文件、数据文件位置

学习怎么找到不同操作系统下，软件不同版本的配置，数据文件应该放置的位置。

### MySQL

[官方文档](https://github.com/docker-library/docs/tree/master/mysql)

#### 需要配置的内容

- root 密码
- 新建账号
- 授权
- 创建数据库

#### 文件位置

- MySQL的配置在文件`/etc/mysql/my.cnf`中指定，这个文件中也包含了`/etc/mysql/conf.d`文件夹中所有以`.cnf`的内容结尾的文件。后面这个文件夹内的配置文件会增强（augment）或覆盖前面的配置。

- 数据文件 `-v /my/own/datadir:/var/lib/mysql`

- 日志文件 `/var/log/mysql/error.log`



##### 推荐的方法

在host上创建配置文件夹，挂载到容器中`/etc/mysql/conf.d`文件夹。

#### 使用DockerHub提供的镜像

查找MySQL镜像`docker search mysql`

`docker pull mysql:5.7`

#### 自己安装


### Redis

### Nginx

### Python


## 精简操作系统

选择适当的操作系统，减小镜像的大小。

### Ubuntu

### CentOS
