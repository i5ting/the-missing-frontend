# the-missing-frontend

![fun.gif](fun.gif)

技术就像这图一样，捅破窗棂纸,将乾坤看个通通透透吧

## 前言

[为什么前端越来越难？越来越有意思？](preface.md)

## 基础

- [了解http-server](docs/httpserver.md)
- 了解MEAN
- 了解phonegap/cordova简史
- 移动端特点
- [如何展望未来的前端](tomorrow.md)
  - js一统天下（nodejs做后端，传统web和h5使用javasctipt，更智能的工具如gulp，更简单的写法如coffeescript等）
  - h5大行其道（网速变快，硬件内存增长）
- [反思一下自己](docs/me.md)
## 前端

js

- jQuery
  - 生疏api如closest，done，defferd等方法
  - 插件写法方法 http://i5ting.github.io/How-to-write-jQuery-plugin/build/jquery.plugin.html
  - 事件（live使用场景，历史，以及on）
  - $.ajax 家谱
  - 如何自己去写一个ajax库 https://github.com/nodeonly/minAjax.js
- Backbone
  - extend
  - 事件
  - mvc
- Angular
  - feature：双向绑定，ioc
  - ioc原理
  - jqlite
  - $q
  - $http
- emberJS 不推荐
- [React](http://facebook.github.io/react/)
- [Underscore.js常用工具卡](http://www.bootcss.com/p/underscore/) or Lo-Dash

css

- bootstrap
- foundation

- 布局
- media query
- sticky css
- CSS Sprite Generator https://css-tricks.com/css-sprites/
- canvas
  - 游戏开发引擎pixi等

模块化加载

- ajax到模块化
- amd/cmd/commonJS
- requirejs/seajs
- 阅读cordova.js代码

Promise/A+规范

- Angular
  - $q
- jQuery
- Nodejs
  - q
  - bluebird
  - async
- iOS/Android

测试

- QUnit

算法，数据结构

设计模式

## h5

boilerplate

- [html5 boilerplate](http://www.bootcss.com/p/html5boilerplate/)


framework

- [jQuery Mobile](http://jquerymobile.com/)
- [Sencha Touch](http://www.sencha.com/products/touch/)

- [ionicframework](ionicframework.com)
- [ratchet](http://goratchet.com/)
- [gmu](http://gmu.baidu.com/)


基于react的空间

- [reapp](reapp.io)


libary

- [zeptojs](docs/zeptojs.md)
  - 兼容jquery api
  - 支持tap等手势
- [iscroll](http://cubiq.org/iscroll-5)
- [fastclick](https://github.com/ftlabs/fastclick)
- [hammer手势](https://github.com/hammerjs/hammer.js)
- [swiper](swiper.com.cn)
- [layer弹出框](http://sentsin.com/layui/layer/)

practice

- [ratchet](http://i5ting.github.io/ratchet-practice/)

## Test

- CasperJS is a navigation scripting & testing utility for PhantomJS and SlimerJS written in Javascript
- tdd/bdd
- http://nodeonly.com/2014/11/24/mongoose-test.html
- mocha
- qunit

## 线上部署


编辑器

https://c9.io/
https://coding.net/home.html

代码片段

http://codepen.io/
http://runjs.cn/

## more

- [todomvc](http://todomvc.com/)
- [awesome-frontend](https://github.com/JingwenTian/awesome-frontend)
- nodejs、express、mocha、mongoose、socket.io
- gulp/grunt
- bower/component
- coffeescript/typescript
- less/sass/scss/stylus
- jade/handlebar/ejs
- markdown编写文档
- github用法
- middleman
- hexo搭建个人博客
- Font Awesome
- Metro UI
- [restfull api](docs/restfull_api.md)
- https://www.npmjs.com/package/v8-profiler
- [发布 / 订阅模式,mq,ws](docs/pubsub.md)
## 八卦

- iojs和nodejs的关系
- grunt与gulp的比较
- node 模块可以在前端使用么？browserify
- 如何看待tdd与debug？
- 是否需要使用IDE？
- [国内上谷歌方法总结](howtogoogle.md)

## FAQ

[faq](docs/faq.md)