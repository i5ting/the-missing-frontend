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



## 如何开发移动应用？


```
最近打算和同学合作开发移动应用，现在的计划是同学用H5开发并打包应用，我用node.js搭建后台。需求大概是这样子：

* 服务器主要实现数据交换和信息实时推送，其他逻辑由应用端实现
* 用户的注册和登录
* 虽然node.js和mongodb是绝配，但最好能支持mysql

我本是做嵌入式方向的，web方向上只用node.js+express搭过简单的网站，所以对C/S的一些概念和开发模式并不熟悉。

我们打算边学边做，最好后期能够小范围上线，所以我们希望从一开始就按照标准、成熟的方案来开发。

那么，希望各位推荐一些node.js后台开发的方案和框架，并且提醒一下零经验开发过程中会忽视或者考虑不到的一些问题。
```


答曰：

1、区分是否是原生应用还是hybrid？

1.1、原生应用开发

express提供json接口即可，然后ios/android通过自己的http库请求该接口

1.2、hybrid应用

区分

- html页面是服务器上
- html页面打包在应用内部，如phonegap的www目录

上面的2种都可以像1.1一样使用json接口，让ui和数据分离，一般如果不是图快得话，都是采用这样的方式

如果第一种，html页面是服务器上，可以使用express + ejs，jade这样模块，可以快速高效的编写h5页面


技术栈推荐

方案1

- bower http://bower.io/ 
- ratchet http://goratchet.com/
- zepto http://zeptojs.com
- fastclick https://github.com/ftlabs/fastclick
- iscroll http://iscrolljs.com
- swiper http://www.swiper.com.cn/

方案2

- jquery mobile（基于jquery 插件简单，缺点定制ui非常麻烦，通过dom属性做绑定，用着恶心）
- ionicframework（基于angular+phonegap的一站式开发框架，足够高大上，学习曲线较高，以后会有可视化界面的）


## node怎么获取远程服务器的时间？

```
要做个功能要求时间不能使用本地时间而是使用某个服务期器上的时间，有什么好的办法么
```

答曰：

    ssh user@ip.com date
    
上面给的是玩的，哈哈

正解

2台服务器，使用ntp同步时间即可

- http://baike.baidu.com/view/60648.htm
- http://blog.chinaunix.net/uid-26454764-id-3230936.html?bsh_bid=210650063


## 升级node版本

首先查看一下本机global模块的依赖是否有问题

```
npm list -g
```


比如报错如下

```
npm ERR! invalid: readable-stream@1.0.33-1 /usr/local/lib/node_modules/phantomjs/node_modules/request/node_modules/bl/node_modules/readable-stream
npm ERR! invalid: browser-launcher@1.0.0 /usr/local/lib/node_modules/testling/node_modules/browser-launcher
npm ERR! extraneous: editor@0.0.6 /usr/local/lib/node_modules/testling/node_modules/browser-launcher/node_modules/editor

```

此时


```
[sudo] npm list -g phantomjs （需要翻墙）
[sudo] npm list -g browser-launcher
[sudo] npm list -g editor
[sudo] npm list -g testling
```

再测试一下

```
npm list -g
```



## 关于 Node.js 项目源码加密

```
最近公司用 Node.js 开发来一款程序, 需要部署在客户的服务器上, 为了防止竞争对手拷贝走源码, 需要对 js 程序进行加密操作.
求各位兄弟给个思路,或者现成的工具.
```

核心逻辑用crypto比较好，大部分还是uglify或者[google的超级变态货closure](https://github.com/google/closure-compiler)