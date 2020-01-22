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
### 打包文件输入输出设置
var path = require('path')
 
//当以命令行形式运行 webpack 或 webpack-dev-server 的时候，工具会发现，我们并没有提供要打包的文件的入口和出口
//此时，他会检查项目根目录中的配置文件，并读取这个文件，就拿出了导出的这个 配置对象 ，然后根据这个对象，进行打包构建
module.exports = {
    entry:path.join(__dirname,'./src/main.js'), // 入口文件
    output:{ //指定输出选项
        path:path.join(__dirname,'./dist'), //输出路径
        filename:'bundle.js'  //指定输出文件
    }
}
### 配置打包命令
dev：webpack-dev-server
<script src="/bundle.js"></script>
访问http：//
bundle.js存在与内存中
```
