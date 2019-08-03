[Github原文链接](https://github.com/geoffgu/interview/blob/master/%E9%9D%A2%E8%AF%95%E5%AE%98%E5%BF%83%E5%BE%97.md)

## js、nodejs 基础

重点考察的部分，基础不好的建议直接拒了，这块没有太大商量余地

* 闭包
* 作用域
* 原型链
* 变量提升
* 函数参数值传递
* this 指向问题
* 函数提升以及优先级问题
* new 操作符做了什么？
* 用 ES5 实现一个继承（有哪些方式）
* 0.2+0.1不等于0.3问题（浮点数精度）
* 堆、栈、队列是什么？都有什么区别？有什么应用？
* 深拷贝、浅拷贝问题（immutable是怎么实现的？）
* typed array 问题
* es6 箭头函数问题
* let 会提升吗？声明、初始化、赋值等概念。什么是暂时性死区？
* 什么是 iterator？for of 用过吗？
* call、apply、bind 区别，bind 怎么实现的？
* caller、callee 了解吗？什么时候会用到？建议用吗？
* es6 其他特性用过吗？（Class、Map、Set、Decorator 等分别考察）
* promise 实现原理（怎么实现取消？怎么实现 promise all、race 等？）
* async await 知识点（await 的作用，async 返回的是什么）
* generator 又是什么？
* v8 线程模型、event loop（async、promise、nextTick、setTimeout、setImmediate 经典问题变着花样考）
* 进程和线程是什么？有什么区别？
* v8 垃圾回收机制
* 输入 URL，浏览器的执行过程又是怎么样的？（浏览器解析方式、顺序，async、defer等）
* 了解前端模块化吗？有几种规范？（commonjs 和 es module 都是怎么实现的？有啥区别？）

## css、html、dom、浏览器相关基础

没什么好说的，前端必修课，样式、html、浏览器相关的不过关建议直接拒了

* 盒模型
* 样式覆盖优先级问题
* 选择器相关问题
* 怎么解决边距重叠？（什么是 BFC？怎么创建 BFC？）
* flex 弹性布局了解吗？用过哪些？（问一些实际问题）
* 移动端的一些坑
* css modules 了解吗？
* sass、less 用过吗？用到了什么特性？实践情况
* 移动端用什么距离单位？（px、百分比、vw、vh、rem 等）
* 什么是逻辑像素，什么是物理像素，设备像素比又是什么？
* 事件捕获冒泡
* 哪些操作导致 reflow、repaint、composite
* 什么时候用 css 动画，什么时候用 transition？选择标准是什么？（如何知道动画执行结束了？）
* dom api 相关
* cookie、localStorage、sessionStorage 区别和使用场景
* 跨域相关问题，怎么解决？几种方式？
* 缓存相关（强缓存、协商缓存，由此引申 http 相关缓存知识）

## 计算机基础

前端对于协议这块必须是要清晰的，如果是 nodejs 团队建议加大难度

* 前端相关网络知识（tcp，dns，cdn，http，https，http2）
* 安全相关（xss、csrf）
* 怎么实现登录的？（cookie based、session based、jwt）
* https 怎么做到防止数据包被拦截的？
* 证书是什么？
* 几种常见加密算法，对称加密、非对称加密

## 设计模式、架构、编程思想

主要考察架构设计能力，软件工程等基本素质，对于资深前端这块有要求

* 用过什么设计模式？怎么实现的？应用场景？
* 项目是怎么做架构设计的？谈谈你的理解
* mvvm 和 mvc 是什么？有啥区别啊
* 函数式和响应式的理解
* 什么是柯里化，怎么实现柯里化？纯函数是啥？
* defineProperty 用过吗？有什么问题？descriptor 是什么？有哪些属性干嘛用的？initializr 是啥？
* 装饰模式了解吗？装饰器用过吗？哪些场景？（高阶组件、es6 decorator）
* 继承和组合用过吗？什么时候用继承什么时候用组合？（mixin 是什么东西？js 是多继承还是单继承？为什么是单继承？）
* 什么是开闭原则？
* 什么是控制反转？什么是依赖注入？
* 什么是面向切面编程
* 你了解的反模式是什么
* 了解尾调用优化吗？通常用在什么场景？js 引擎有做这层优化吗？什么是尾递归？

## 数据结构、算法相关（easy 难度）

对于前端来说考到 easy 难度差不多了（我自己也是个弱鸡~）

数据结构比如树、链表相关的在前端应用界是常用的，建议考察

图论、动归、线段树、蓄水池抽样等这种根据自己的业务领域来决定是否有必要考察（=. =，web 前端我感觉不需要）

* 大 O 表示法，怎么计算时间复杂度和空间复杂度
* 贪心算法是什么？动态规划是什么？（背包、爬楼梯、金矿问题）
* 实现一个记忆化的斐波那契数列
* 求并集、交集
* 链表相关（排序、合并、去重）
* 树相关（对称二叉树、翻转二叉树、前中后序遍历、深度广度优先遍历、递归非递归实现）

## 智力题

主要考察反应速度、逻辑思维、推理能力，达到正常以上水平即可

* 25 匹马
* 烧绳子
* 推理题

## 应用框架原理

考察是不是只会用，只是技术栈的罗列，而不清楚内部的原理机制，更没有借鉴落地的场景，这块也是重点考察

* react、angular、vue 实现原理（三个选一个候选人最擅长的，针对某个流程详细考察，比如 dom diff、dom patch、脏检查、双向绑定、依赖收集等）
* setState 相关问题，dirty component 是啥
* forceUpdate() 用过吗？是什么干嘛用的？与 setState 有啥区别？
* props 和 state
* 组件设计相关（怎么设计？受控和非受控是什么？）
* children.map 是什么，和普通的 map 有什么区别？使用场景
* cloneElement 干嘛用的，使用场景，和 createElement 区别
* 生命周期相关
* react 16 新特性，react 17 前瞻，fiber，hooks，suspense，异步渲染等
* redux、mobx、vuex、dva 等状态管理框架实现原理，针对几个点详细考察
* redux 或 mobx 怎么处理 side effect？
* redux 中间件模型，thunk 怎么实现？saga 怎么实现的？
* koa、express 用过吗？中间件模型了解吗？有啥区别？
* router 用过吗？核心流程怎么实现的？
* 用过什么 xhr 封装库？（axios、fetch，各家长短？有啥坑吗？）
* babel 原理（有哪些东西，分别干嘛用的，怎么实现的，runtime，polyfill，register）
* webpack 核心流程原理，怎么实现模块化的，treeshaking 怎么做的？

## 其他

随便问点一些业务上的思考，技术加分项，或技术视野、分享、选型方面的考虑

* 使用 typescript 吗？如何看待的，什么情况下用，类型声明文件怎么写的
* 单元测试（jest、mocha、ava）
* 如何发布一个二方或三方包，有哪些考量
* 技术选型的考量指标、维度
* mongo、es、redis 方面相关知识
* 工程化、ci、docker、k8s 相关知识

<!-- > 大概就这些，持续更新......

如果有兴趣来酷家乐，可以找我内推，我的邮箱：feifan@qunhemail.com -->