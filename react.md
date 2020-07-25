
# React.js-第1天

## 1.React简介

+ React起源于Facebook的内部项目，因为该公司对市场上所有JavaScript MVC框架，都不满意，就决定自己写一套，用来架设Instagram (照片交友)的网站。做出来以后，发现这套东西很好用，就在2013年5月开源了。
+ 由于React的设计思想极其独特，属于革命性创新，性能出众，代码逻辑却非常简单。所以，越来越多的人开始关注和使用，认为它可能是将来Web开发的主流工具。
+ 清楚两个概念:
  + library (库) :
  + Framework (框架) :

## 2.前端三大主流框架

+ Angular.js: 出来较早的前端框架，学习曲线比较陡，NG1学起来比较麻烦，NG2 ~ NG5开始，进行了一系列的改革，也提供了组件化开发的概念;从NG2开始，也支持使用TS (TypeScript) 进行编程;
+ Vue.js: 最火的一门前端框架，它是中国人开发的，对我我们来说，文档要友好一 些;
+ React.js: 最流行的一门框架，因为它的设计很优秀;



## 3.React与vue的对比

### 组件化方面

1. 什么是模块化：

2. 什么是组件化：

3. 组件化的好处：

4. Vue是如何实现组件化的：通过.vue文件创建组件
   template 结构
   style 样式
   script 行为
5. React如何实现组件化：

### 开发团队方面

+ React是由FaceBook前端官方团队进行维护和更新的；因此，React的维护开发团队，技术实力比较雄厚；
+ Vue第一版，主要是有作者尤雨溪专门进行维护的，当Vue更新到2.x版本后，也有了一个以尤雨溪为导的开源小团队，进行相关的开发和维护;


### 社区方面

+ 在社区方面，React由于诞生的较早，所以社区比较强大，一些常见的问题、坑、最优解决方案、文档、博客在社区中都是可以很方便就能找到的；

+ Vue是近两年才火起来的，所以，它的社区相对于React来说，要小一些，可能有的一些坑，没人踩过；

### 移动APP开发体验方面

+ Vue, 结合Weex这门技术，提供了迁移到移动端App开发的体验(Weex， 目前只是一个小的玩具， 并没有很成功的大案例；)

+ React,结合ReactNative,也提供了无缝迁移到移动App的开发体验(RN用的最多，也是最火最流行的) ;

## 4.为什么要学习React

1. 和Angular1相比，React设计很优秀，一切基于JS并且实现了组件化开发的思想;

   React中一切都是以js来表现的，包括style样式

2. 开发团队实力强悍，不必担心断更的情况;

3. 社区强大，很多问题都能找到对应的解决方案;

4. 提供了无缝转到ReactNative.上的开发体验，让我们技术能力得到了拓展;增强了我们的核心竞争力;
5. 很多企业中，前端项目的技术选型采用的是React.js;

## 5.React中几个核心的概念


### 虚拟DOM (Virtual Document Object Model)

+ **DOM的本质是什么**：浏览器中的概念，用JS对象来表示页面上的元素,并提供了操作DOM对象的APl;
+ **什么是React中的虚拟DOM**: 用JS对象来模拟页面上的DOM和DOM嵌套;

+ **为什么要实现虚拟DOM (虚拟DOM的目的) **: 为了实现页面中，DOM元素的高效更新

+ **DOM和虚拟DOM的区别**:
  + **DOM**:
  + **虚拟DOM**:

### Diff算法

+ tree diff
+ component diff
+ element diff

Before

After

\6. JkM4Jwebpack4.xIE

需求:点击列头，实现表格排序
1、表格中的数据从哪儿来，从数据库查询来
2、这些查询到的数据存放到哪儿了，存放在浏览器的内存中，并且是以对象数组的方式存放
3、这些数据是怎么渲染到页面上的
 手动for循环，拼接字符串，如jsp的方式
 使用模板引擎，如art-template
4、思考:上述的方案，有没有性能上的问题?

;5如果用戸点毒了[咐同] ,想安装肘祠M大到小排序:

1.触麦点去事件.在事件中，把内存中的 対象数埋.重新排序;

z.当排完序之后,両面是旧的;但是内存中的対象数組是新的;

3.想か法,把暴新的数組,重新渣染到頁面上: (有没有性籠 上的何題)
一个网页呈现的过程:
1、浏览器请求服务器获取HTML代码
2、浏览器需要先在内存中，解析DOM结构，并在内存中，渲染出一棵DOM树
3、浏览器把DOM树，呈现到页面上 



### 12.深入理解Store、Action、Reducer
