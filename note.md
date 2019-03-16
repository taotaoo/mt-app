# 环境准备
* 安装node，npm
* 安装nrm，将npm的源更换为淘宝源。`nrm use taobao`
* 安装webpack。`npm i -g webpack``
* 安装vue
* 初始化nuxt工程
  ```
  npm i -g npx
  npx create-nuxt-app mt-app
  ```
* 使用babel解决es2015语法问题
    * 在package.json中的启动命令中增加`--exec babel-node`
    * 增加.babelrc文件，中内容`{"presets": ["es2015"]}`
    * 安装依赖 `npm i babel-preset-es2015`


* 增加支持scss
    * `npm i sass-loader node-sass`

* 启动mongo
    * `docker run -d --name mongo -v /Users/wangxin/1.learning/mongo:/data/db -p 27017:27107 mongo`

* 安装redis
    * `docker run -p 6379:6379 -v $/Users/wangxin/1.learning/redis:/data  -d redis:3.2 redis-server --appendonly yes`