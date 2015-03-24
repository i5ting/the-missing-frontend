# 如何展望未来的前端

我先告诉未来很美好，你先做好准备。然后慢慢的等我聊聊。

## 4个时期

界面技术从上世纪DOS字符界面到Windows图形界面（或图形用户界面GUI），Browser浏览器界面，移动端应用4个不同的发展时期

1. Terminal终端
1. GUI图形用户界面
1. Browser浏览器
1. Mobile移动端

我们在以web开发来细分

1. Browser（曾经无数时间我们都在兼容ie）
1. Mobile Browser（html5）

不管你承认与否，现在都是移动互联网时代

## 2个变革的桥梁都是浏览器


### 从c/s到b/s架构的演变

直白点讲就是：从GUI到Browser的架构演变。

要想对“C/S”和“B/S”技术发展变化有所了解，首先必须搞清楚三个问题。

第一、什么是C/S结构。

C/S（Client/Server）结构，即大家熟知的客户机和服务器结构。它是软件系统体系结构，通过它可以充分利用两端硬件环境的优势，将任务合理分配到Client端和Server端来实现，降低了系统的通讯开销。目前大多数应用软件系
统都是Client/Server形式的两层结构，由于现在的软件应用系统正在向分布式的Web应用发展，Web和Client/Server应用都可以进行同样的业务处理，应用不同的模块共享逻辑组件；因此，内部的和外部的用户都可以访问新的和现有的应用系统，通过现有应用系统中的逻辑可以扩展出新的应用系统。这也就是目前应用系统的发展方向。
传统的C／S体系结构虽然采用的是开放模式，但这只是系统开发一级的开放性，在特定的应用中无论是Client端还是Server端都还需要特定的软件支持。由于没能提供用户真正期望的开放环境，C/S结构的软件需要针对不同的操作系统系统开发不同版本的软件，加之产品的更新换代十分快，已经很难适应百台电脑以上局域网用户同时使用。而且代价高，效率低。

第二、什么是B/S结构。

B/S（Browser/Server）结构即浏览器和服务器结构。它是随着
Internet技术的兴起，对C/S结构的一种变化或者改进的结构。在这种结构下，用户工作界面是通过WWW浏览器来实现，极少部分事务逻辑在前端
（Browser）实现，但是主要事务逻辑在服务器端（Server）实现，形成所谓三层3-tier结构。这样就大大简化了客户端电脑载荷，减轻了系统维护与升级的成本和工作量，降低了用户的总体成本（TCO）。
以目前的技术看，局域网建立B/S结构的网络应
用，并通过Internet/Intranet模式下数据库应用，相对易于把握、成本也是较低的。它是一次性到位的开发，能实现不同的人员，从不同的地
点，以不同的接入方式（比如LAN,WAN,Internet/Intranet等）访问和操作共同的数据库；它能有效地保护数据平台和管理访问权限，服
务器数据库也很安全。特别是在JAVA这样的跨平台语言出现之后，B/S架构管理软件更是方便、快捷、高效。

第三、B/S相比C/S的优势

B/S结构下软件相比C/S结构下软件，有着独特的优势。

节约投资。B/S结构下软件一般只有初期一次性投入成本；而C/S结构下软件则随着应用范围的扩大，要求不断进行资本的投入。比如需要购买更为高级的服务器或者增加相应的管理人员等。

简化工作。B/S结构下软件安装在服务器端即可解决问题，在做更改时，只需调整服务器端即可。C/S结构下软件则需要安装在客户机端，调整的时候需要涉及到局域网内的每一台机器。对于区域级服务器来讲，C/S结构的软件更新则更加复杂。

更好地保障数据安全。在C/S结构软件的解决方案里，对于异地经营的大型集团企业，需要在各地分别安装区域级服务器。一旦某一个区域级服务器出现问题，对数据的安全会造成一定影响，而且总部也不会得到准确的最终数据。对B/S结构下软件来讲，其数据集中存在于企业的中央数据库，可有效地保护数据的安全，而且企业可随时随地掌握自己的经营状况、市场动态，以做出最快决策。

不受网络的限制。C/S结构软件仅适用于局域网内部用户或宽带用户（1兆以上）；而B/S结构软件则适合于任何网络结构（包括28.8K拨号入网方式），尤其适合于宽带不能达到的地方。

### 从传统web到html5的hybrid开发演变

传统web开发就不多讲了，相信大部分人都明白。

#### 移动应用开发分类

- native原生开发
- Hybrid混搭开发


native原生开发指的使用移动设备上系统支持的语言开发的app，比如android使用java开发，iOS使用oc开发，最终开发的应用以apk和ipa包得形式上传到应用商店，提供给移动设备进行安装。


Hybrid混搭开发是指使用html5技术开发的跨浏览器应用，并最终可以将html5.js.css等打包成apk和ipa包的开发方式。它也可以上传到应用商店，提供给移动设备进行安装。它最大的好处是通过h5开发一次，就可以在多个平台上安装。

Hybrid App主要以JS+Native两者相互调用为主，从开发层面实现“一次开发，多处运行”的机制，成为真正适合跨平台的开发。目前已经有众多Hybrid App开发成功应用，比如百度、网易、街旁等知名移动应用，都是采用Hybrid App开发模式。
经过众多开发者与成功案例证明Hybrid App兼具了Native App的良好用户体验的优势，也兼具了Web App使用HTML5跨平台开发低成本的优势。现在有更多的开发者在面临移动平台的选择，所以在这里根据开发中各个平台的使用情况，针对现在主流的平台进行分析。

#### 主流移动平台分析

Hybrid App开发，现阶段主流的平台包括PhoneGap，AppCan，appMobi，Titanium等，它们基于webkit开源内核，使用HTML5 标准开发，适配机型简单，支持开发者自定义插件，并能很好的应用于商业，教育，娱乐等行业，成为移动开发者的首选开发平台。

#### 总结

从上面的描述，我们可以知道Hybrid混搭开发是通过移动端浏览器为核心，作为界面和操作系统间交互的媒介。

## h5特点

- 语义化表情
- css3动画
- media query
- canvas
- cache：localstorage,websql ,indexdb
- 其他移动端特性，如陀螺仪，地图等

## 未来的2点

- js一统天下（nodejs做后端，传统web和h5使用javasctipt，更智能的工具如gulp，更简单的写法如coffeescript等）
- h5大行其道（网速变快，硬件内存增长）

## 总结

前端开发人员有更多可以尝试和学习的机会，这是机遇也是挑战。加油吧，前端er们。

我们的时代到了
