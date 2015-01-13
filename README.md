# grunt-livereload-demo

 利用grunt-contrib-connect 与 grunt-contrib-watch 当监测指定文件被`增加`,`改变`,`删除`时，执行预定义任务

### 运行方法
`npm install`

安装依赖的包

`grunt demo`

运行grunt的demo 任务

`grunt dev`

运行grunt的dev 任务


###相关参数：

####files
监测的文件路径和名称
可以是字符串，也可以为数组

####tasks
当文件状态发生改变后，执行的任务列表

#### options.spawn
默认值：`ture`

是否在子进程中运行spawn 任务

####options.interrupt
默认值：`false`

当文件发生修改，这个监测任务，会spawn 任务在子进程，默认的行为是，当上一个进程结束时，才会为每一个目标新建一个子进程，设置为true的时候，一旦发生更改，立刻打断上一个进程，直接新建一个

####options.debounceDelay
支持类型：`integer`

默认值：`500`

文件发生更改后，再次发生同样事件所需要的间隔，注：有时候习惯多按几次保存，这其中的间隔

####options.event
支持类型：String|Array

默认值：ALL

追踪文件更改的事件类型all,changed,added,deleted

####options.reload
支持类型：`Boolean`

默认值:`false`

当设置为true,每次更改文件，都会restart watch task,非常常用于，Gruntfile 依赖于其他文件
设计一个配置文件的watch任务，当配置文件发生改变时，重置watch tasks

####options.atBegin
支持类型:`Boolean`

默认值:`false`
这个选项可以触发所有监测事件当watch开始的时候

####options.livereload
TYPE：`Boolean|Number|Object`

Default:`false`
可以自动刷新页面，当css,或者图片等发生变化


