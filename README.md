# vue-docker

> use windows npm

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

> use centos7 docker

前提：已经通过windows npm run build打包项目，生成dist

## 下载Nginx image

$ docker pull nginx

## 编写Dockerfile

$ touch Dockerfile  创建空文件(不需要手动创建，git上已经建立)

$ cd /home/vue-develop/project

$ git clone https://github.com/qingjie1201/vue-docker.git

$ 通过命令copy 最新dist到/home/vue-develop/project/vue-docker目录下

## Docker打包

$ cd /home/vue-develop/project/vue-docker

$ docker build -t vue-docker .

$ docker build -t myproject/vue-docker-example:v0.0.1 .  基于Dockerfile构建新镜像(仓库/名称)

$ docker build -t myproject/vue-docker-example:v0.0.1 /home/vue-develop/project/vue-docker

## Docker运行

$ docker run -d --name vue-docker -p 9000:9000 vue-docker

$ docker run -d --name vue-docker -p 9000:9000 myproject/vue-docker-example:v0.0.1

## 查看运行结果

$ docker ps

访问 http://192.168.0.227:9000
