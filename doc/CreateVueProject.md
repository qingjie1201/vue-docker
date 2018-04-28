# CreateVueProject

创建Vue项目

## 搭建环境

window系统、cmd命令、安装有 Node.js、 vue、 vue-cli

### 安装node.js

本机: soft\开发工具\node-v8.2.1-x64.msi

官网下载地址：https://nodejs.org/en/

设置淘宝镜像：大家都知道国内直接使用 npm 的官方镜像是非常慢的，这里推荐使用淘宝 NPM 镜像

npm install -g cnpm --registry=https://registry.npm.taobao.org

### 安装webpack

cnpm install -g webpack

### 安装vue脚手架

npm install -g vue-cli

cd D:\vue-develop\project cd 目录路径 创建vue项目

## 创建Vue项目

vue init webpack <projectName> 如 vue init webpack vue-docker

cd D:\vue-develop\project\vue-docker

npm install 或者 cnpm install 下载依赖

npm run dev 运行项目

访问 http://localhost:8080

创建好项目后，可以使用WebStorm打开项目，进行开发

npm install -g yarn

yarn dev
