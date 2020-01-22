# vueReadMe
## 1.wepack
```
//包初始化
npm init -y
//安装webpack
npm i webpack webpack-cli -D
//新建webpack.config.js文件，添加如下内容
module.exports={
    mode:'development'//mode决定打包速度和大小
}
//package.json新增属性
script中的"dev": "webpack"
//打包
rpm run dev
//生成dist/main.js
//引入js
<script src="../dist/main.js"></script>

```
