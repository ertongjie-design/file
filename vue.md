#####2.18 vue-resource发起get、post、jsonp请求
#####2.19 结合Node手写JSONP服务器剖析JSONP原理
4.JSONP的实现原理
+ 由于浏览器的安全性限制，不允许AJAX访问协议不同、域名不同、端口号不同的数据接口，浏览器认为这种访问不安全
+ 可以动态添加script标签，通过script标签的src属性指向数据接口地址，因为script标签不存在跨域限制，这种数据获取方式，称作jsonp(注意：根据jsonp的实现原理，可知，jsonp只支持get请求)

5.小知识点

+ 使用cnpm install -g nodemon后在nodemon打开服务端
+ \== 对于数据类型可以自动转换，比较不严格  ===对数据类型有要求

##### 3.6动画
动画制作步骤：
1、使用transition元素，把需要被动画控制的元素包裹起来，该元素是Vue官方提供
2、自定义两组样式，来控制transition内部的元素实现动画
css实现效果要操作dom，vue就是要不操作dom实现效果
v-enter、v-leave-to、v-enter-active、v-leave-active

#####3.16创建组件的方式

#####小知识点
cnmp是npm的国内镜像
安装node服务器运行命令nodemon的命令：cnpm install -g nodemon

#####问题
1、
2、3.6动画没看懂

#####英语
prefix：前缀
opacity:不透明度

webpack是前端的一个项目构建工具，它是基于Node.js开发出来的一个前端工具

nrm是一个基于node的包管理工具

axios是请求后台资源的模块
可以调用axios,发起异步请求

vue-cli 是vue.js的脚手架，用于自动生成vue.js模板工程

Element-Ul是饿了么前端团队推出的一款基于Vue.js 2.0 的桌面端UI框架，手机端有对应框架是Mint UI 

Ssh:strusts+spring+hibernate

SSM:springmvc+spring+mybatis

MyBatis 是一款优秀的持久层框架，本质是对jdbc的封装整合，前身是ibatis。

Spring Cloud 是致力于分布式系统、云服务的框架，是在SpringBoot基础之上构建的快速开发分布式系统的工具集

Dubbo是一个分布式服务框架

Spring是一个开源的轻量级的Java开发框架。简化应用程序的开发，体现在Ioc、Aop、声明式事务

Spring Boot是由Pivotal团队提供的全新框架
目的是用来简化Spring应用的创建、运行、调试、部署等。
使用Spring Boot可以做到专注于Spring应用的开发，而无需过多关注XML的配置
用了springboot就不用配置Spring的xml配置文件

SpringMVC是Spring框架的一个子框架、模块,是基于mvc的webframework模块。
mvc是一种设计模式，即model-view-controller

Redis是数据库的一种

Nginx是一个使用c语言开发的高性能的http服务器及反向代理服务器

node.js 是一个基于 Chrome V8 引擎的 JavaScirpt 运行环境，是一个服务端的js。
前端的JavaScript其实是由ECMAScript、DOM、BOM组合而成
BOM是一些操作浏览器的方法

webpack是web前端模块化构建工具

vuex是什么：vuex是一个专门为vue.js开发的状态管理模式
vuex做什么：采用集中式存储管理应用的所有组件的状态，并以相应的规则保证状态以一种可预测的方式发生变化。
			原本共享状态更新需要组件之间通讯，现在每个组件是和store进行通讯，对于大型项目管理组件的状态十分有效，
			小项目还是使用HTML5自带的localStorage和sessionStorage作为数据传递

vue是什么：vue是一款轻量级js框架
vue做什么：分离数据和视图，利用虚拟dom降低真实dom频繁排版与重绘的消耗
发布时间：2016.05发布vue.js 2.0、2019.10发布vue.js 3.0

Jquery封装了dom操作，让对dom的查询更简便，所以在vue中不要用Jquery
正则表达式全局替换 /单纯/g
格式字符串，tab上的那个符号，用法：`${变量}-${变量}-${变量}`
原生JS需要写在vue的后面
虚拟dom不会进行排版与重绘操作，它只是一个JavaScript Object
虚拟dom是在内存中维护的dom树，是在实体dom上的一层抽象
内存中有个dom树，dom元素要想渲染到页面上，首先要放进内存中的dom树中
获取焦点是dom元素的方法，元素还未放进dom中去的时候，不是dom元素
浏览器的渲染引擎会解析元素

click：
keyup：
keydown：
mouseup：
mousedown：

数组push：用于在数组后方添加新的对象
数组unshift：用于在数组前方添加新的对象
数组some：用于遍历数组。用法：list.some((item,i)=>{}),return true就会停止some的循环
数组splice：分离内容出去，两个参数，一为分离起始点，二为分离个数。返回未被分离的内容
数组findIndex：找到位置，返回出去。用法：list.findIndex(item => {}),同样返回true停止循环
数组forEach：遍历每一个数据。用法：list.forEach(item => {})
数组filter：return需要的值，方法自动将返回的值添加到数组中并返回出去
字符串indexOf：返回参数字符串在调用方法字符串中的位置，没有则是-1。可用于检测包含与否
字符串includes：包含与否
字符串replace：替换指定字符，返回值为替换结果，只替换一个。第一个参数还可写正则
字符串toLowerCase：
[es6]字符串padStart：第一个参数为长度，第二个参数为填充内容。
[es6]字符串padEnd：第一个参数为长度，第二个参数为填充内容。
Date对象getFullYear：
Date对象getMonth：返回数字，从0开始
Date对象getDate：返回号数
Date对象getDay：返回星期几
Date对象getHours：
Date对象getMinutes：
Date对象getSeconds：
数字toString：

第一天：
1、mvc和mvvm的区别
mvc是后端概念，是从整个项目的角度考虑的
mvvm是前端概念，vm是核心，是m和v的连接者，提供数据绑定

2、插值表达式、v-cloak、v-text、v-html

3、v-if和v-show
通过其中属性值为true或false改变元素展示状态
当为false时，v-if的元素被移除，有较高的切换性能消耗，若元素不会被展示出来，则使用if
v-show的元素设置为display:none，有初始渲染消耗，若元素展示状态切换多，则用show

4、v-bind、v-on、v-for、v-mode
v-bind用于将属性值识别为变量，可用:代替，通常使用可以双向交换数据的v-model
使用：<p v-bind:class="msg"></p>
通过v-bind有两种绑定样式的方式，class和style

v-on简写为@，用于绑定事件，v-on的事件值中不一定写方法名，还可以进行对数据的操作

v-for的使用：简单数组
<p v-for="(item, i) in list">索引值：{{i}} --- {{item}}</p>
data: {
			list: [1,2,3,4,5,6]
}
v-for的使用：包含对象的数组
<p v-for="item in list">索引值：{{item.id}} --- {{item.name}}</p>
data: {
			list: [
			{id:1, name: "zs1"}
			{id:2, name: "zs2"}
			{id:3, name: "zs3"}
			{id:4, name: "zs4"}	
			]
}
v-for的使用：遍历对象
<p v-for="(val, key) in list">索引值：{{val}} --- {{key}}</p>
data: {
			list: {id:1, name: "zs1"}
}
v-for的使用：迭代数字
<p v-for="count in 10">索引值：{{count}}</p>
data: {
}
注意：迭代的数字从1开始
key用于将dom元素和对应数据绑定起来，但注意key属性的值应该是字符串或数字，并且key应和v-bind一起使用

v-mode只能用于表单元素

5、事件修饰符：.stop 阻止冒泡 .prevent 阻止默认行为 .capture 捕获机制 .self 阻止自己被冒泡 .once 只执行一次
用法：@click.prevent="方法名"
按键修饰符：用法同事件修饰符 .enter .esc .delete .space .tab .up .down .left .right
可写按键码，有所有的按键，即数字，但不好记。可以自定义全局按键修饰符Vue.config.keyCodes.变量 = 按键码

6、vm实例中的属性概念
el：指定要控制的区域
data：是个对象，指定数据
methods：是个对象，自定义方法
要访问data中的数据或methods中的方法需要用到this

第二天：
1、过滤器
作用：调整文本格式，做输出前最后一层处理。
可用于插值表达式或v-bind处，插值表达式后加 | 和过滤器名字
过滤器调用采用就近原则
过滤器分全局过滤器和自定义局部过滤器

2、自定义指令
v-mode、keyup这些都是指令，内置指令
vue中所有的指令调用时都以v-开头
使用Vue.directive()定义全局指令，参数1是指令名称，定义时指令名称前不需要加v-前缀；
指令后传值需要区分字符串和变量
实际指令中binding.name  .value .expression
参数2是个对象，对象中有方法，方法格式bind:function(el){el.focus()}，还有inserted元素插入dom之后执行、update是VNode更新后
方法参数第一个永远是el，表示被绑定了指令的那个dom元素
bind是在刚绑定指令的时候执行，这时元素还没有插入到dom中去，调用focus方法无效，bind时放置属性可以，进入页面创建时不会清除
属性用bind，方法行为用inserted
自定义指令不能放在script最下面

3、生命周期函数
----组件创建时期
创建vue实例对象
初始化事件和生命周期（生命周期有些相关的函数）
第一个：beforeCreate（创建前），表示实例完全被创建出来之前，会执行它。这个时期，data和methods中的数据、方法都还没有被初始化
初始化数据和方法（改为初始化注入和校验）
第二个：created（已创建），data和methods中的数据、方法已经被初始化
（第二个和第三个生命周期函数之间的内容都是在进行模板的编译，把vue代码中的那些指令执行）
（最终在内存生成一个编译好的最终模板字符串，然后把这个模板字符串渲染为内存中的dom，还没挂载到页面）
是否有el
是否有template	否：将el对应的html编译为模板
第三个：beforeMount（挂载前），此时，页面中的元素还没有被替换，还只是模板字符串，如插值表达式会原样输出
将内存中的模板挂载到页面上去
第四个：mounted（已挂载），用户可以看到渲染好的页面，这是vm实例创建期间的最后一个生命周期函数，
该函数执行完代表实例已经被完全创建好，组件脱离创建阶段
如果某些插件要操作页面上的dom节点，最早要在mounted中进行

----组件运行时期
data中的数据发生改变
第一个：beforeUpdate（更新前），此函数中查看，data数据改变，但页面上的内容未改变
虚拟dom重新渲染并应用更新，虚拟dom就是内存中的dom树
	根据data中最新的数据，重新渲染出一份最新的内存dom树，当内存dom树被更新后，会把最新的内存dom树，重新渲染到真实的页面去，
	就完成了从data（Model层） -> view（视图层）的更新
第二个：updated（更新后），页面上的内容已改变

----组件销毁时期
调用vm.$destoryed()函数
第一个：beforeDestory（销毁前），当执行该函数，vue实例就从运行阶段进入到销毁阶段，浏览器窗口关闭就销毁。
	这时实例身上所有的data和所有的methods以及过滤器、指令还处于可用状态，还未真正执行销毁过程
执行销毁，解除绑定
第二个：destoryed（销毁后），此时，组件已经被完全销毁，组件中所有的过滤器、指令、数据、方法都不可用

4、vue-resource实现get、post、jsonp请求
常见的数据请求类型：get、post、jsonp
vue-resource依赖于vue，因此vue-resource需要放在vue后
有了vue-resource后在vue实例上添加了一个$http属性
这个vue的插件提供了使用XMLHttpRequest或JSONP发送Web请求和处理响应的服务
通过this.$http.get().then(successCallback,errorCallback)发送get请求，成功的回调必须有，失败的回调是可选的
then获取服务器返回的数据，一看到.then就要知道这个方法是用promise来封装的，promise是解决回调地狱的
get(url, [config])、jsonp(url, [config])、post(url, [body], [config])：body是要发送给服务器的数据对象{}，
跨域问题
resource在vue2就不再维护
手动发起的post请求默认没有表单格式，有的服务器处理不了





1、vue项目中如何设置点击后改变样式
2.--hot代表啥
3，2.18中说
4，open如何知道默认打开哪个浏览器的
5，-S和-D有什么区别
6，
7、main和组件中导入的有啥区别
8、我在这个组件里使用的数据和方法还需要export default暴露出去吗
9、对于js文件和vue文件的关系很懵
10、




手机知识点
class是ES6中提供的新语法，用来实现ES6中面向对象编程的方式
函数的本质就是对象
静态属性，实例属性
webpack中默认只能处理es6的一些语法，更高级的es6甚至es7语法需要通过第三方loader转换为低级的，拿给webpack打包到bundle.js中
npm run dev运行整个文件
markdown编辑器haroopad

webpack-dev-server --open --port 3000 --hot
其中open代表默认打开浏览器，

2.18vue-resource发起get、post和jsonp请求
Shift+home

6.6webpack中babel的配置(安装)

通过Babel，是个可以帮助我们将高级语法转换为低级语法的loader
1、在webpack中可以通过执行如下两套命令，安装两套包，去安装Babel相关的loader功能
1.1第一套包:cnpm i babel-core babel-loader babel-plugin-transform-runtime -D
babel-plugin-transform-runtime这是一个Babel的插件，名称不包含前面的babel-plugin-
第一套包是babel的转换工具
1.2第二套包:cnpm i babel-preset-env babel-preset-stage-0 -D
第二套包是语法，高级es和低级es的关系映射
2.打开webpack的配置文件，在module节点的rules数组中，添加一个新的匹配规则
2.1
{test:/\.js$/,use:'babel-loader',exclude:'node_modules'}
2.2注意:在配置babel的loader规则的时候，必须把node_modules目录，通过exclude选项排除掉，原因有两
2.2.1如果不排除node_modules，Babel会把node_modules中的所有第三方js文件都打包编译，会非常消耗cpu同时打包会很慢
2.2.2哪怕Babel把node_modules中所有的js都转换完成，项目也无法运行
3.在项目的根目录中新建一个名叫.babelrc的Babel配置文件，这个文件属于JSON格式，因此在写.babelrc配置的时候必须符合JSON规范，如不写注释，字符串必须用双引号
3.1在Babel配置中写如下内容
{
  "presets":["env","stage-p"]
  "plugins":["transform-runtime"]
}
json文件中不支持注释
webpack官方文档
匹配规则=loader规则=loader配置项
Babel配置文件的内容也可在webpack配置文件中配置
Babel已到8
Babel的安装去babel官网cv两下就好
报错就去装包
npm下载不到7.0版本上的babel-core
新版本的stage-x废掉了，不用装

6.7关于babel的一点说明
babel-preset-env是最新的语法插件，包含了所有的es***语法

6.8使用vue实例的render方法渲染组件
有时候使用 npm i node-sass -D，就必须使用cnpm i node-sass -D
组件的模板对象
如果想在页面上以标签的形式引入组件，需要在vm实例的components属性上注册一下
render属性render:function(createElements){
  return createElements(模板名称)
}
createElements是一个方法，调用它能把指定的模板对象渲染成html结构，会替换el指定的容器。render返回的是一个虚拟的dom节点Vnode

6.9区分webpack中导入vue和普通网页使用Script导入vue的区别
如何在webpack构建的项目中，使用vue进行开发
npm i vue -s(把vue这个包安装为项目运行依赖)
import Vue from 'vue'(包名)
'vue'包是在node_modules中找的
此处字符串中可写要导入的js的相对路径
通过这种方式导入的Vue构造函数只提供runtime-only的方式
回顾包的查找规则:
1.在项目根目录中查找有没有node_modules文件夹
2，在node_modules中根据包名，找到对应的vue文件夹
3，在vue文件夹中，找一个叫package.json的包配置文件
4，在package.json文件中，查找一个main属性，main属性指定了当外界require或import
包的入口文件，通过修改这个值，修改要导入的内容
node_modules在vscode中隐藏了
项目根目录和node_modules的vue下都有package.json
package.json中默认使用的是vue.runtime.common.js
把main.js和网页连接起来的是在webpack的配置文件webpack.config.js中配置的了入口文件
module.exports={
  entry:path.join(__dirname,'./src/main.js')，
  resolve:{
    alias:{
      'vue$':'vue/dist/vue.js'
代表导入时以vue结尾的找这个
路径默认就是在node_modules目录下
}
}
}
./和没有是一样的，都代表相对当前路径
修改配置文件要重新启动

6.10在vue中结合render函数渲染指定的组件到容器中
main.js中导包更改也要重启
runtime-only的vue的模板编译器不可用
现在runtime-only的vue的模板编译器可用了
.vue就是一个纯粹的组件，分三部分
1.<template>写html代码
2.<script>写业务逻辑
3.<style>写样式
一个组件里只能有一个根元素
因为包体积小所以要用runtime-only的vue
创建vm实例是在main.js中
按照路径导入组件即整个vue
vue-cli需要webpack的原理
webpack无法打包.vue文件，需要安装相关的loader，npm i vue-loader vue-template-compiler -D
vue-loader内部依赖vue-template-compiler
安装好loader后需要在webpack的配置文件中写loader配置项
{test:/\.vue$/,use:'vue-loader'}
test是匹配什么类型的文件，use是指用哪个loader来处理
用于处理vue文件
使用的一种服务器渲染技术，降低浏览器的负载，最后发布项目的时候浏览器可以直接渲染内容，不需要编译模板
模板对象被vue组件文件取代，直接import那个组件，只需要import这一个
components被render取代
当vue-loader在15版本以上需要和VueLoaderPlugin一起
匿名函数即function关键字后直接跟参数的函数
可以改造为箭头函数，去掉function,在参数和大括号中间加=>，若参数只有一个，可以去掉参数的括号
render中的createElements方法名称可以随意
函数中只有一行代码可以省略大括号，省略大括号后默认就return，因此return也不需要

6.11webpack结合vue使用的总结
1、安装vue的包cnmp i vue -S
2、由于在webpack中推荐使用.vue这种模板对象组件，因此需要安装能解析这种文件的loader,，npm i vue-loader vue-template-compiler -D
3、在main.js中，导入vue的模块，import Vue from 'vue'(包名)，因为import的是构造函数，因此最好大写即Vue
4、创建一个.vue结尾的组件，组件分三部分template script style 
5、使用 import login from './login.vue'导入这个组件
6、创建vm实例，var vm = new Vue({el:"#app",render:c=>c(login)})
7、在页面中创建一个id为app的元素作为我们vm实例要控制的元素
第2步后还应需要在webpack的配置文件中配置loader配置项

6.12export default 和 export的使用方式
组件中的data必须是个函数,数据通过returrn出来
Node中向外暴露成员的形式，module.exports={}
暴露使用module.exports或exports，获取使用var 标识名称 = require('模块标识符')
es6中也通过规范的形式规定了es6中如何导入导出模块
es6中导入模块使用import 模块名称 from '模块标识符'  import '表示路径'
模块标识符就是文件路径
es6中使用export default 和 export向外暴露成员
export default 向外暴露的成员可以使用任意变量来接受
export default 只可向外暴露一次
export向外暴露的成员只能使用相同变量来接受，在{}里面，可使用as改名，叫做按需导出

6.13结合webpack使用vue-router
main中一import自定义组件，实际拿到的是vue-loader将该.vue文件处理得到的最终的模板，是三个标签结合得到的最终的对象
PowerShell窗口，cnpm i 先装包20个，装完node_modules就出来了
安装.vue插件后，输入//就可以快速输入vue模板代码
Alt+f4快速跳转到脚手架使用教程
安装cnpm i vue-router -S
之前通过src安装
1，在模块化工程中必须导入包后通过，Vue.use(VueRouter)
2，先导入account组件对象
3，创建路由对象var router = new Router({
  routes:[
{path:'/account',component:account}
]
})
4，挂载到vm实例上
app组件是通过render渲染出来的
render会清空覆盖，因此不要把router-link和router-view写在vm控制的容器中
放在render渲染的那个组件里面去
router-link会改变地址中hash值，依据其path中的值，然后地址改变被路由监听到，去路由列表routes里找符合的组件渲染出来
render也是占坑，不过这个坑是通过vm实例的el指定的容器

6.14结合webpack实现children子路由
代码提示装包vetur,vue 2 snippets
子路由的path不以/开头
子路由点击后的地址会连接父路由的地址
真正开发都是写组件和路由

6.15组件中style标签lang属性和scoped属性
scoped属性使样式不冒泡，默认要冒泡
style标签默认只能使用普通样式格式输入,想用less或scss，需要在style标签中添加lang属性指定需要的样式格式。
scss语法:样式格式是嵌套

6.16抽离路由模块

7.1scoped属性选择器的实现原理
属性选择器是在标签选择器的后面加中括号，括号中跟属性名。
加了scoped的style的那个组件，其根标签会被vue自动加上一个属性。

7.2Mint-UI中按钮组件的使用
Mint-UI和bootstrap完全不同，Mint-UI是基于vue.js，bootstrap不是基于vue.js的。
Mint-UI是移动端组件库。bootstrap不是组件库是代码片段。
element UI是桌面端的
vue2.0安装mint-ui是npm install mint-ui -S要简写，不行换cnpm
和vue-router使用方式相同
完全导入浪费bundle.js中的空间
推荐按需导入组件，然后通过Vue.component(组件.name,组件)将组件注册到全局
导入mint-ui中的样式库，import 'mint-ui/lib/style.css'，可以省略node_modules,因为会自己去里面找
全局导入需要导入样式文件，按需导入不需要
去官方查看组件详细信息
Vue.use(MintUI)就是将所有组件注册为全局组件

7.3Mint-UI中Toast组件的使用
在app组件中编辑，要按需导入组件，是js组件
官网中自行查找
vue中的this指的组件实例
bootstrap自带图标
外部的package.json中写的依赖，可以看安装了哪些组件
在main.js中直接import字符串
bootstrap4不直接支持glyphicon，可以使用open-iconic
使用箭头函数可以改变作用域

7.4Mint-UI按需导入组件
借助于babel-plugin-component
官方npm install babel-plugin-component -D,实际cnpm install babel-plugin-component -D
修改.babelrc
按需导入的和自己写的都是通过Vue.component进行注册，注册可指定组件名称，可通过名称在html中写此标签

7.5介绍MUI
MUI不同于Mint-UI，MUI只是开发出来的一套好用的代码片段，提供了配套的样式和配套的html代码段，类似于bootstrap。Mint-UI是真正的组件库，是使用vue技术封装出来的成套的组件，可以无缝的和vue项目进行集成开发。
任何项目都可以使用MUI和bootstrap,Mint-UI只适用于vue项目
Vue.use和Vue.component区别应该在于use是整个组件库，component是个别组件
为啥官方的安装指令都和实际的不同，官方都是npm install，实际都是cnpm i,还带后缀
MUI不能使用npm下载，需要手动去github上下载github.dcloudio.mui
dist目录中是发布出来的产品

7.6MUI的使用
node_modules目录是用npm装的所有第三方包，src/lib下是手动加入的第三方包
导样式组件这些都是在main中

7.7项目-vue项目演示

7.8项目-整理出一个基本的项目模板

7.9项目-制作项目首页的Header和Tabbar区域
在js中操作数据库相当于直接把数据库权限给用户
文件夹中按哪个键就一下子跳到那个键开头的

7.10项目-把本地项目托管到码云中
项目管理工具:svn,git
README.md是告知项目相关信息的
开源项目都有一个开源协议LICENSE
git init创建本地仓储产生.git文件夹，报错去配置环境变量
git status 查看当前文件提交状态
git add . 此时还未提交
git commit

7.11项目-使用vs code默认集成的Git工具快速提交代码

7.12项目-完成tabbar的小图标设置

7.13项目-完成路由链接的改造和路由高亮
选中后使用ctrl+d，继续选中其他相同的内容








p38 新的接口地址
http://www.liulongbin.top:3005/api/getlunbo
http://www.liulongbin.top:3005/api/post
http://www.liulongbin.top:3005/api/jsonp

http://三达不溜.liulongbin.top:3005，用这个域名替代http://vue.studyit.io就可以请求到数据了(｡･ω･｡)

获取列表地址:  http://www.liulongbin.top:3005/api/getprodlist/
添加地址:  http://www.liulongbin.top:3005/api/addproduct/
删除地址:  http://www.liulongbin.top:3005/api/delproduct/

跟着视频做的项目地址：https://github.com/galenjx/vue-cms 
里面有完成的项目和我在这个项目遇到的问题与解决方案，包括webpack4.x，babel7.x配置，新的可用接口，相关插件api更新等等问题

跟着视频做的项目地址:https://gitee.com/studyLi/heima/tree/master

loader报错看这个https://github.com/vuejs/vue-loader/issues/1238

真实项目实战GitHub地址：https://github.com/ragnar-document/leaveSoundMass-project/blob/master/README.md
技术栈：node/vue/小程序/axios/封装思想

node写的后端服务器，模仿p40-p44的接口，地址： https://www.jianshu.com/p/c56eea972457

vue写的仿网易云音乐网站
http://www.shanshihao.cn
源码在这：https://github.com/sl1673495/vue-netease-music

107P报错的解决方案：
// 通过Babel，可以帮我们将高级的语法转换为低级的语法
// 在终端中 npm install -D babel-loader @babel/core @babel/preset-env webpack
// 还有 npm i @babel/plugin-proposal-class-properties -D
// 然后在配置文档中的loader节点中加入
// {
//     test: /\.m?js$/,
//     exclude: /(node_modules|bower_components)/,
//     use: {
//       loader: 'babel-loader'
//     }
// }
//在根目录创建一个.babelrc文档，里面的内容为
// {
//     "presets": ["@babel/preset-env"],
//     "plugins": ["@babel/plugin-proposal-class-properties"]
// }
g：表示全局（global）模式，即模式将被应用于所有字符串，而非在发现第一个匹配项时立即停止；
i：表示不区分大小写（case-insensitive）模式，即在确定匹配项时忽略模式与字符串的大小写；
m：表示多行（multiline）模式，即在到达一行文本末尾时还会继续查找下一行中是否存在与模式匹配的项。

2019年6月25日 18:28:32
现在已经是webpack4.35
默认安装的是4.35
npm uninstall webpack
先卸载了之前安装的4
npm i webpack@3.* -g
安装webpack3配合教学使用，减少坑。
如果安装了4
编译的时候要加上-o参数用来输出编译后的文件位置 加上 --mode development来设置环境
后面你会发现除了webpack，其他配套的也升级版本了，不如就去适应webpack4
关于webpack4，在黑马的react教程里的0.9节里有关于4的讲解

时间：2020/2/19   webpack版本：4.41.6
P93中的webpack.config.js配置文件这样写就可以直接用webpack命令：const path=require('path');
module.exports ={
    entry:'./src/main.js',
    output:{
        path:path.resolve(__dirname,'dist'),
        filename:'bundle.js'
    }
}

https://www.bilibili.com/video/BV1e7411j7T5?p=4
webpack4

webpack真的麻烦安装各种版本的babel。老是报错。然后看了一下别人的项目文件。安装低版本的css-loader。终于解决了。

webpack4的安装方法
https://www.cnblogs.com/wo1ow1ow1/p/11451235.

这个视频的完整教学和课堂代码链接：https://pan.baidu.com/s/18j4s_LWxKq6hbjUH-xDFTA 
提取码：05qr

vscode的代码提示插件Aixcoder

https://gitee.com/vsdeveloper/vue110/tree/master

建议严格按照一下版本安装各种插件.... 
 "devDependencies": {
    "babel-core": "^6.26.0",
    "babel-loader": "^7.1.2",
    "babel-plugin-transform-runtime": "^6.23.0",
    "babel-preset-env": "^1.6.1",
    "babel-preset-stage-0": "^6.24.1",
    "css-loader": "^0.28.7",
    "file-loader": "^1.1.5",
    "html-webpack-plugin": "^2.30.1",
    "less": "^2.7.3",
    "less-loader": "^4.0.5",
    "node-sass": "^4.5.3",
    "sass-loader": "^6.0.6",
    "style-loader": "^0.19.0",
    "url-loader": "^0.6.2",
    "webpack": "^3.8.1",
    "webpack-dev-server": "^2.9.3"
  },

知乎web实战vue适合入门地址：https://github.com/ragnar-document/ZhihuWeb

SpringBoot+Vue+Element-UI (新冠-物资管理系统) 前后端分离项目， 抗疫相关物料的管理系统，领用、派发记录，库存查询统计。寂寞消遣之作~, 项目预览地址：https://www.zykhome.club

你们key使用对象也不报错的原因是因为使用了vue.min.js，压缩版把错误提示 去掉了



vuex重点在于集中式存储管理，看浏览器收藏
vuex集成到 Vue 的官方调试工具 devtools extension中，提供诸如零配置的 time-travel 调试、状态快照导入导出等高级调试功能
，其中不提倡操作dom元素