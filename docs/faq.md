# FAQ


## Node是不是要比Rails折腾啊?

学Rails一个框架就够了,Node下有Express, Koa,还有Meteor,Rails只用学一个,学Node要学仨?

答曰：

```
会一个就可以了，为啥一直折腾

express会了再说。koa还早，是下一代，至于metetor适合开发实时应用，亲何苦都学了呢?

话在说回来，就是3个加一起也没有一个rails大，

express = sinatra
koa = express
Meteor 也不大
说概念类似，可以看一下sails

```


## 求：运维后台系统开发教程

没有node开发经验。想要入门做这么一套系统：
能批量调用linux服务器上的脚本、执行系统命令、显示执行过程、监控系统状态、告警、上传文件。
请问有教程推荐一个吗？谢谢了！

答曰：

- shell.js(页面里执行命令)
- npm shelljs(执行命令)
- express + multer（web service和上传）

以上足够了



## ng里怎么让你想起java了?

mvc模式最早是smalltalk里的，java里最初是swing里用得，不想没有成功，结果在web开发上火了。从ejb到servlet演进，2004年Martin Fowler总结了ioc相关经验，Rod Johnson(Spring框架的作者)写了《Expert One-on-One J2EE Development without EJB》。。。。。

所以你看ng得时候

- mvc
- ioc
- 指令（类似jsp里的taglib）
- 双向绑定（struts等框架里都有）

那么，熟悉java的亲们，看到ng会想到什么呢？

## mocha 的 README。。。。无聊吐槽。。。

```
我满怀期待地打开，里面除了开发者再无所有。。。。无语。。。。怎么看。。。。
```


   
亲，它有官网好么？哈哈

少抱怨，多思考，未来更美好


## 部署nodejs一般用什么工具。？

pm2:http://www.douban.com/note/314200231/


## mongoose的翻译

mongoose的翻译是猫鼬。。。

![](https://dn-cnode.qbox.me/Fr4o_k4R6435GWNxToeentuGNFAp)


##  npm不是全局安装的么,怎么放在版本控制里?

```
npm install -g
```

才是全局的，而

```
npm install --save
```
这是本地装的，你可以在当前目录看到node_modules目录

用git做版本控制的时候`npm init` 和`express .`会产生`.gitignore`文件，此文件了默认忽略了node_modules目录，所以你提交的时候是没有node_modules的。

从积极的角度看，是需要忽略的，尽可能和最新的模块保持一致，俗话见追涨不追跌

