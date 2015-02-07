# grunt-livereload-demo

 利用[grunt-contrib-connect](https://github.com/gruntjs/grunt-contrib-connect) 与 [grunt-contrib-watch](https://github.com/gruntjs/grunt-contrib-watch) 当监测指定文件被`增加`,`改变`,`删除`时，执行预定义任务
 
## 开始

假如你没有使用过 [Grunt](http://gruntjs.com/) , 确保学习完 [Getting Started](http://gruntjs.com/getting-started) 向导, 它解释了如何创造一个 [Gruntfile](http://gruntjs.com/sample-gruntfile) 和如何安装与使用一个grunt插件

### 安装
`npm install`

安装依赖的包

### 运行

`grunt server`

运行grunt的`server` 任务

`grunt server1`

运行grunt的`server1`任务

`ctrl + c`

暂停运行的任务

###相关提示：

`livereload`在watch和connect中,都需要设置，并且对应的值需要一致
`hostname`为`*` 可以使局域网中，任意设备通过ip访问
`base`的路径是相对项目的根目录
