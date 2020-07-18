首先非常感谢所有我遇到的人, 没有你们就没有现在的我, 我会继续向上的, 大家共同进步。
# Front-end-interview-questions

> 简介: 根据本人自己的面试经历, 总结的一套算是全面的面试题及答案。有什么不对的地方请多批评指教, 谢~。

## 前端
```
1.HTML
    html跟html5有啥区别？
        文档声明: 
            html: 超文本标记语言, 一种纯文本类型的语言。
            html5: 文档声明HTML5方便书写, 精简, 有利于程序员快速的阅读和开发。
        结构语义区别: 
            html: 没有体现结构语义化的标签, 如: <div id="nav"></div>。
            html5: 添加了许多具有语义化的标签, 如: <article>、<aside>、<audio>、<bdi>...。
        绘图区别: 
            html: 指可伸缩矢量图形, 用于定义网络的基于矢量的图形。
            html5: HTML5的canvas元素使用脚本(通常使用JavaScript)在网页上绘制图像, 可以控制画布。
        html: 主要用于PC端开发使用。
            优点: 
                1. 开发过程中前端与后端脱离, 交互通过JSON传输来实现。
                2. 跨平台能力更强, 依托于浏览器的支持。
            缺点:
                1. 开发难度大, 考虑浏览器的兼容性。
                2. 无法直接显示java实体类对象, 需要转换为json格式。
        html5: 主要用于wap端开发使用。
            优点: 
                1. 摆脱对平台的依赖: 
                    HTML5可以让你摆脱对平台的依赖, 用户打开浏览器, 直接就可以访问你的应用, 而不需要经过各种Store的审核。
                2. 实时更新: 
                    实时更新, 通常平台的审核都需要七个工作日左右的时间, Web方式就不存在这种问题。
                3. 离线使用: 
                    用户可以离线使用, 更新下载量及少, 可以全部更新, 也可以选择替换部分文件。
            缺点: 
                1. 完善性方面: 许多特性各种浏览器的支持程度不一样。
                2. 技术门槛方面: HTML5简化开发者工作的同时, 代表有许多的属性和API需要开发者学习, 像web, worker, web socket等。
                3. 性能方面: 某些平台下的引擎问题导致HTML5性能低下。
    html5有什么新标签？
        video: 表示一段视频并提供播放的用户界面.
        audio: 表示音频.
        canvas: 表示位图区域.
        svg: 定义矢量图.
        nav
        header
        aside
        article
        template
        section
        footer
        ...
        参考文档: https://www.w3school.com.cn/html5/html5_reference.asp

2.CSS
    css跟css3有啥区别？
        css: 
            1. 是一种用来表现HTML, XML等文件样式的计算机语言。
            2. 不仅可以静态地修饰网页, 还可以配合各种脚本语言动态地对网页各元素进行格式化。
            3. 能够对网页中元素位置的排版进行像素级精确控制, 支持几乎所有的字体字号样式, 拥有对网页对象和模型样式编辑的能力。
        css3: 
            1. 是css(层叠样式表)技术的升bai级版本。
            1. 主要包括盒子模型, 列表模块, 超链接方式, 语言模块, 背景和边框, 文字特效, 多栏布局等模块。
            3. 新特征有很多, 例如: 圆角效果, 图形化边界, 块阴影与文字阴影, 使用RGBA实现透明效果, 渐变效果, 使用@Font-Face实现定制字体, 多背景图, 文字或图像的变形处理(旋转, 缩放, 倾斜, 移动), 多栏布局, 媒体查询等。
    css3有什么新属性？
        animation: 动画效果.
        transform: 变换效果.
        transition: 过渡效果.
        box-shadow: 阴影效果.
        text-shadow: 文本阴影.
        word-wrap: 自动换行.
        border-color: 为边框设置多种颜色.
        border-image: 图片边框.
        border-radius: 圆角边框.
        background-clip: 指定背景图片从什么位置开始裁剪.
        background-size: 指定背景图片尺寸.
        background-origin: 指定背景图片从哪里开始显示.
        ...
        参考文档: http://css.cuishifeng.cn/
    css都有那些选择器？
        1.标签选择器
        2.id选择器
        3.类选择器
        4.组选择器
        5.通配符选择器
        6.后代选择器
        7.子类选择器
        8.伪类选择器
    说一下css的权重？
        !important > 行内style > id > 类、伪类、属性 > 类型、伪元素 > 通配 > 浏览器自定义或继承的
    display都有那些属性？
        none: 元素不会被显示.
        block: 元素将显示为块级元素, 元素前后会带有换行符.
        inline: 元素会被显示为内联元素, 元素前后没有换行符.
        inline-block: 行内块元素.
        table: 元素会作为块级表格来显示, 类似<table>, 表格前后带有换行符.
        table-row: 元素会作为一个表格行显示, 类似<tr>.
        table-cell: 元素会作为一个表格单元格显示, 类似<td>和<th>.
        ...
        参考文档: http://css.cuishifeng.cn/display.html
    px跟rem、em之前的计算区别？
        px: 是我们网页开发常用的像素, 是图像的基本采样单位。
        em: 指相对于父元素的字体大小的单位。(相对单位)相对于父元素 div { font-size: *px } 1rem = *px; 例: div { font-size: 14px } 1rem = 14px;
        rem: 指相对于根元素的字体大小的单位。(相对单位)相对于html { font-size: *px } 1rem = *px; 例: html { font-size: 16px } 1rem = 16px;
        注: 
            1. 320px是移动端最小限制像素。
            2. 一般用: html { font-size: 16 × (当前设备宽度 ÷ 320)  + 'px' }
3.原生js
    简单的说一下你理解的面向对象？
        万物皆对象, 把一个对象抽象成类,具体上就是把一个对象的静态特征和动态特征抽象成属性和方法,也就是把一类事物的算法和数据结构封装在一个类之中,程序就是多个对象和互相之间的通信组成的.
        面向对象具有封装性,继承性,多态性。
        封装:隐蔽了对象内部不需要暴露的细节,使得内部细节的变动跟外界脱离,只依靠接口进行通信.封装性降低了编程的复杂性. 
        通过继承,使得新建一个类变得容易,一个类从派生类那里获得其非私有的方法和公用属性的繁琐工作交给了编译器. 而继承和实现接口和运行时的类型绑定机制
        所产生的多态,使得不同的类所产生的对象能够对相同的消息作出不同的反应,极大地提高了代码的通用性.
        总之,面向对象的特性提高了大型程序的重用性和可维护性.
    null和undefined的区别？
        null: (没有对象)
            1. 作为函数的参数, 表示该函数的参数不是对象。
            2. 作为对象原型链的终点。
        undefined: (缺少值)
            1. 定义了形参, 没有传实参, 显示undefined。
            2. 对象属性名不存在时, 显示undefined。
            3. 函数没有写返回值, 即没有写return, 拿到的是undefined。
            4. 写了return, 但没有赋值, 拿到的是undefined。
        null和undefined转换成number数据类型: 
            1. null 默认转成 0
            2. undefined 默认转成 NaN
    什么是原型？什么是原型链？原型跟原型链有啥区别？
        原型: 在JavaScript中, 原型也是一个对象, 原型的作用, 则是实现对象的继承。在js的所有函数对象中, 都存在一个属性prototype, 该属性对应当前对象的原型。
        原型链: 原型链是有一些用来继承和共享属性的对象 组成的对象链。并且原型链的长度是有限的。
        区别: 在层级多的关系中, 多个原型层层相连则构成了原型链。在查找一个对象的属性时, 倘若在当前对象找不到该属性, 则会沿着原型链一直往上查找, 直到找到为止, 如果到了原型链顶端, 还没找到, 则返undefined。
    什么是作用域？什么是作用域链？作用域跟作用域链有啥区别？
        作用域: (代码执行开辟栈内存)
            1. 私有作用域 ----> 函数执行都会形成一个私有作用域。
            2. 全局作用域 ----> 页面一打开就会形成一个全局的作用域。
        作用域链: (作用域形成的链条: 当代码在一个环境中执行时, 会创建变量对象的一个作用域链)
            1. 作用域链的前端, 始终都是当前执行的代码所在环境的变量对象。
            2. 作用域链中的下一个对象来自于外部环境, 而在下一个变量对象则来自下一个外部环境, 一直到全局执行环境。
            3. 全局执行环境的变量对象始终都是作用域链上的最后一个对象。
        区别: 内部环境可以通过作用域链访问所有外部环境, 但外部环境不能访问内部环境的任何变量和函数。
    说一下你理解的闭包？
        闭包: 
            1. 闭包是指有权访问另一个函数作用域中的变量的函数。
            2. 可以在函数的外部访问到函数内部的局部变量。 
            3. 让这些变量始终保存在内存中, 不会随着函数的结束而自动销毁。
        优点: 
            1. 可访问函数内部的变量, 防止变量污染作用域(隐藏变量), 从而实现封装。
        缺点: 
            2. 会增加内存的开销, 需注意防止内存泄漏。
        注意: 
            1. 由于闭包会使得函数中的变量都被保存在内存中, 内存消耗很大, 所以不能滥用闭包, 否则会造成网页的性能问题, 在IE中可能导致内存泄露。解决方法是, 在退出函数之前, 将不使用的局部变量全部删除。
            2. 闭包会在父函数外部, 改变父函数内部变量的值。所以, 如果你把父函数当作对象(object)使用, 把闭包当作它的公用方法(Public Method), 把内部变量当作它的私有属性(private value), 这时一定要小心, 不要随便改变父函数内部变量的值。
    js循环机制的原理？
        1. 整体 script 作为第一个宏任务进入主线程, 遇到 console.log, 输出 script start。
        2. 遇到 setTimeout, 其回调函数被分发到宏任务 Event Queue 中。
        3. 遇到 Promise, 其 then函数被分到到微任务 Event Queue 中,记为 then1, 之后又遇到了 then函数, 将其分到微任务 Event Queue 中, 记为 then2。
        4. 遇到 console.log, 输出 script end。
    js的浅拷贝跟深拷贝？
        拷贝: 就是把父对像的属性, 全部拷贝给子对象。
        浅拷贝: (缺点: 如果父对象的属性等于数组或另一个对象, 那么实际上, 子对象获得的只是一个内存地址, 而不是真正拷贝, 因此存在父对象被篡改的可能) 
            1. for
            2. for in
            3. forEach
            ...
        深拷贝: 
            1. 递归(递归调用浅拷贝)
            2. 转换成字符串对象JSON.stringify()
            ...
    说一下你开发中常见的兼容性问题都是怎么解决的？
        1. 阻止浏览器默认行为: return false。
        2. 取消默认事件
            w3c: e.preventDefault();
            IE: e.returnValue = false;
        事件注意点: 
            1. event代表事件的状态, 例如触发event对象的元素, 鼠标的位置及状态, 按下的键等等。
            2. event对象只在事件发生的过程中才有效。
            3. firefox里的event跟IE里的不同, IE里的是全局变量, 随时可用; firefox里的要用参数引导才能用, 是运行时的临时变量。
            4. 在IE/Opera中是window.event, 在Firefox中是event; 而事件的对象, 在IE中是window.event.srcElement, 在Firefox中是event.target, Opera中两者都可用。
    简述你理解的原生Ajax的步骤？
        1. 创建ajax对象
            var xhr = new XMLHttpRequest();
        2. 设置回调函数(根据需求是否需要此步骤)
            xhr.onreadystatechange = function(){ ... };
        3. 设置请求地址以及请求方式(ajax下的open方法)
            xhr.open('get', 'http://www.github.com');
            第一个参数为请求方式, 第二个参数为请求地址/服务器端对应的路由请求地址
        4. 设置请求头(根据需求是否需要此步骤)
            xhr.setRequestHeader("Content-Type","application/x-www-form-urlencoded");
        5. 发送请求
            xhr.send();
        6. 获取服务器端与客户端的响应数据
            xhr.onload = function () {
                // xhr.responseText 获取服务器端的响应数据
                console.log(xhr.responseText);
            }
4.Es6
    es6都有什么新特性？
        1. 箭头函数 (() => {})
        2. 解构赋值 const obj = { name: '', sex: '' }; const { name, sex } = obj;
        3. 函数参数默认值 const foo = function (name = '', sex = '') {};
        4. 字符串拼接 `我的姓名是${name}, 性别${sex}`
        5. let 新增的块级作用域, 不能重复声明, 可重新赋值的变量
        6. const 新增的块级作用域, 不能重复声明, 不可重新赋值的常量
        ...
    es5跟es6有啥区别？
        es5: 是ECMAScript第五个版本
            1. strict模式
                严格模式, 限制一些用法, 'use strict';
            2. Array增加方法
                1. 增加了every, some , forEach, filter , indexOf, lastIndexOf, isArray, map, reduce, reduceRight方法
                2. 还有其他方法 Function.prototype.bind, String.prototype.trim, Date.now
            3. Object方法
                Object.getPrototypeOf
                Object.create
                Object.getOwnPropertyNames
                Object.defineProperty
                Object.getOwnPropertyDescriptor
                Object.defineProperties
                Object.keys
                Object.preventExtensions / Object.isExtensible
                Object.seal / Object.isSealed
                Object.freeze / Object.isFrozen
                注: 只讲有什么, 不讲是什么。
            ...
        es6: ECMAScript6在保证向下兼容的前提下, 提供大量新特性
    普通函数跟箭头函数有啥区别？
        区别: 
            1. 写法不同
            2. 当前this指向不同
        普通函数: 
            1. 在箭头函数出现之前, 每个新定义的函数都有其自己的 this 值
            2. 在ECMAscript5中将this赋给一个变量来解决 var foo = function () { var that = this } 除此之外, 还可以使用 bind 函数, 把期望的 this 值传递给需要用的函数
        箭头函数: 
            1. 箭头函数会捕获其所在上下文的 this 值, 作为自己的 this 值
            2. 箭头函数不绑定arguments, 取而代之用 rest 参数...解决 var foo = (...args) => { return args[0] }
            3. 箭头函数不能用作构造器, 和 new 一起用就会抛出错误。var Foo = () => {}; var foo = new Foo(); //Foo is not a constructor
            4. 箭头函数没有原型属性。var foo = () => {}; console.log(foo.prototype) //undefined
5.Node.js
    说一下require.js的特点？说一下Sea.js的特点？require.js跟sea.js有啥区别？
        require.js: 
            执行的AMD规范, 所有的依赖模块都是限制性, 当然require.js从2.0开始, 也改成可以延迟执行(根据写法不同, 处理方式不同)。这点和常规的node.js风格很像, 模块编写前把所有用到的依模块率先在头部注入进来, 然后需要调用的时候就可以直接拿来用。require.js会先尽早地执行(依赖)模块, 相当于所有的require都被提前了, 而且模块执行的顺序也不一定100%先model1再model2。因此你看 执行顺序和你预想的完全不一样。
        sea.js: 
            执行的CMD规范, sea.js只会在真正需要使用(依赖)模块时才执行该模块, sea.js是异步加载模块的没错, 但执行模块的顺序也是严格按照模块在代码中出现(require)的顺序, 这样也许更符合逻辑。sea.js对模块的态度是懒执行的, 这样有四个好处: 
                1.防止对象被提前创建(内存优化, 如加载plist文件等耗内存的操作)
                2.防止对象重复创建(永远只加载一次)
                3.防止对象使用时, 还没被创建
                4.可以在懒加载方法里面, 进行初始化操作
6.Vue
    说下Vue的生命周期？
        实例化: new Vue()
        创建前: beforeCreate()
        创建后: created()
        载入前: beforeMount()
        载入后: mounted()
        更新前: beforeUpdate()
        更新后: update()
        销毁前: beforeDestroy()
        销毁后: destroyed()
    简述下Vue双向绑定的原理？
        1.实现一个监听器Observer, 用来劫持并监听所有属性, 如果有变动的, 就通知订阅者。
        2.实现一个订阅者Watcher, 每一个Watcher都绑定一个更新函数, watcher可以收到属性的变化通知并执行相应的函数, 从而更新视图。
        3.实现一个解析器Compile, 可以扫描和解析每个节点的相关指令(v-model, v-on等指令), 如果节点存在v-model, v-on等指令, 则解析器Compile初始化这类节点的模板数据, 使之可以显示在视图上, 然后初始化相应的订阅者(Watcher)。
    简述下Vue-Router路由的原理？
        通过改变 URL, 在不重新请求页面的情况下, 更新页面视图。因为js可以实时获取地址栏的信息, 所以vue利用这一点, 用js动态的去控制页面的展示模块, 由当前页面切换到下一个页面。hash可以获取地址栏'#'后面的参数, 利用History interface在html5中新增的方法。在vue-router中通过mode这一参数控制路由, 从而更新页面。
    说一下Vue-Router有那些钩子？
        导航被触发, 在失活的组件里调用离开守卫, 调用全局的 beforeEach 守卫, 在重用的组件里调用 beforeRouteUpdate 守卫, 在路由配置里调用 beforEnter, 解析异步路由组件, 在被激活的组件里调用beforeRouteEnter, 调用全局的 beforeResolve 守卫, 导航被确认, 调用全局的 afterEach 钩子, 触发 DOM 更新, 在创建好的实例调用 beforeRouteEnter 守卫中传给 next 的回调函数。
        // 前置守卫
        router.beforeEach((to, from, next) => {
            // do someting
        });
        // 后置钩子
        router.afterEach((to, from) => {
            // do someting
        });
        // 独享钩子
        beforeEnter: (to, from, next) => {
            // do someting
        }
        // 组件内的导航钩子
        beforeRouteEnter(to, from, next) {
            // do someting
            // 在渲染该组件的对应路由被 confirm 前调用
        },
        // 组件内的导航钩子
        beforeRouteUpdate(to, from, next) {
            // do someting
            // 在当前路由改变, 但是依然渲染该组件是调用 
        },
        // 组件内的导航钩子
        beforeRouteLeave(to, from ,next) {
            // do someting
            // 导航离开该组件的对应路由时被调用
        }
    vue-cli跟webpack有啥区别？
        webpack: 是一个前端资源的打包工具, 它可以将js、image、css等资源当成一个模块进行打包。
            中文官方网站: https://www.webpackjs.com/
            好处: 
                1. 将许多碎小文件打包成一个整体, 减少单页面内的衍生请求次数, 提高网站效率。
                2. 将ES6的高级语法进行转换编译, 以兼容老版本的浏览器。
                3. 将代码打包的同时进行混淆, 提高代码的安全性。
            教程: (主要的几个说明)
                1. 安装webpack, webpack支持全局安装和本地安装, 官方推荐是本地安装 $ npm install webpack --save-dev
                2. 核心概念: 入口(entry), 输出(output), 加载器(loader), 插件(plugins)
                3. 编写webpack配置
                4. 执行打包 webpack xxx.js
                5. 测试运行
                6. 热更新的web服务等(可自行完善webpack配置)
        vue-cli: 在开发中, 需要打包的东西不止是js、css、html。还有更多的东西要处理, 这些插件和加载器如果我们一一去添加就会比较麻烦。vue官方提供了一个快速搭建vue项目的脚手架: vue-cli, 使用它能快速的构建一个web工程模板。
            官网: https://github.com/vuejs/vue-cli
            教程: 
                1. 安装 $ npm install -g vue-cli
                2. 项目结构
                3. 单文件组件
                4. 运行
        区别: 
            webpack是一个前端的打包工具, vue-cli是一个快速构建工程的脚手架, 包含了不止打包文件。
    什么是单页面应用？单页面应用的优缺点？
        单页面应用, 就是只有一张web页面的应用。单页应用程序是加载单个html页面并在用户与用于程序交互时动态更新该页面的web应用程序。浏览器一开始会加载必需的html、css和javaScript, 所有的操作都在这张页面上完成, 都由javaScript来控制。因此对单页面应用来说模块化的开发和设计显得相当重要。
        速度: 
            更好的用户体验, 让用户在web app感受native app的速度和流畅。
        MVC: 
            经典MVC开发模式, 前后端各负其责。
        ajax: 
            重前端, 业务逻辑全部在本地操作, 数据都需要通过AJAX同步、提交。
        路由: 
            在URL中采用#号来作为当前视图的地址,改变#号后的参数, 页面并不会重载。
            因为单页面应用上的所有操作都在这一张页面上完成, 这一切的所有也都是由javaScript来控制。因此单页面应用上会包含大量的javaScript代码。
        优点: 
            1. 分离前后端关注点, 前端负责界面显示, 后端负责数据存储和计算, 各司其职, 不会把前后端的逻辑混杂在一起。
            2. 减轻服务器压力, 服务器只用出数据就可以, 不用管展示逻辑和页面合成, 吞吐能力会提高几倍。
            3. 同一套后端程序代码, 不用修改就可以用于Web界面、手机、平板等多种客户端。
        缺点: 
            1. SEO问题, 现在可以通过Prerender等技术解决一部分。
            2. 前进、后退、地址栏等, 需要程序进行管理。
            3. 书签, 需要程序来提供支持。
    什么是mvc？什么是mvvm？mvc跟mvvm有啥区别？
        mvc: (model、view、controller)
            单向通讯
            优点: 
                1. 模块化
                2. 复用性
            缺点: 
                1. 使用mvc会增加代码量、相应的也会增加软件开发的成文, 设计的难度也会增加。
         mvvm: (model、view、viewModel)
            自动同步
            优点: 
                1. 低耦合: View可以独立于Model变化和修改, 同一个ViewModel可以被多个View复用；并且可以做到View和Model的变化互不影响。
                2. 可重用性: 可以把一些视图的逻辑放在ViewModel, 让多个View复用。
                3. 独立开发: 开发人员可以专注与业务逻辑和数据的开发ViewModemvvmdi计人员可以专注于UI(View)的设计。
            缺点: 
                1. bug很难调试, 如果看到界面异常, 有可能是view中的代码有bug, 也有可能是model中的代码有bug。数据绑定使得一个位置的bug快速传递别的位置, 要定位原初始问题就变得不那么容易了。
                2. 一个大的模块中model也很大, 虽然使用方便了也很容易保证数据的一致性, 但当长时间持有, 不释放内存就造成了花费更多的内存。
                3. 数据双向绑定不利于代码重用。客户端开发最常用的就是view, 但是数据双向绑定技术, 让你在一个view中都绑定了一个model, 不同模块的model都不同, 那就不能简单重用view了。
        注: mvvm是在mvc的基础上开发出来的。
7.Angular
    说一下Angular的生命周期？
        1. 初始化: constructor()
        2. 载入页面数据发生改变: ngOnChanges()
        3. 数据发生改变后初始化: ngOnInit()
        4. 检测是否有数据变化: ngDoCheck()
        5. 调用其他组件后只初始化一次: ngAfterContentInit()
        6. 调用其他组件后有数据发生变化时: ngAfterContentChecked()
        7. 其他组件视图及子组件视图展示后初始化: ngAfterViewInit()
        8. 每次做完组件视图和子视图的变更检测之后调用: ngAfterViewChecked()
        9. 组件销毁: ngOnDestroy()
    简述下Angular双向绑定的原理？
        1、每个双向绑定的元素都有一个watcher
        2、在某些事件发生的时候, 调用digest脏数据检测。
            这些事件有: 表单元素内容变化、Ajax请求响应、点击按钮执行的函数等。
        3、脏数据检测会检测rootscope下所有被watcher的元素。
            $digest函数就是脏数据监测。
            Angular 在 scope 模型上设置了一个监听队列, 用来监听数据变化并更新 view 。每次绑定一个东西到 view 上时 AngularJS 就会往 $watch 队列里插入一条 $watch , 用来检测它监视的 model 里是否有变化的东西。当浏览器接收到可以被 angular context 处理的事件时,  $digest 循环就会触发, 遍历所有的 $watch , 最后更新 dom。
8.React
    说一下React的生命周期？
        1. 挂载
            constructor()
            static getDerivedStateFromProps()
            render()
            componentDidMount()
        2. 更新
            static getDerivedStateFromProps()
            shouldComponentUpdate()
            render()
            getSnapshotBeforeUpdate()
            componentDidUpdate()
        3. 卸载
            componentWillUnmount()
9.小程序
    说一下小程序的生命周期？
        组件的生命周期: 
            1. 创建时执行: created()
            2. 进入页面节点树时执行: attached()
            3. 组件视图层布局完成后执行: ready()
            4. 组件实例被移动到节点树另一个位置时执行: moved()
            5. 组件实例被从页面节点树移除时执行: detached()
            6. 每当组件方法抛出错误时执: error()
        组件在页面的生命周期: 
            1. 组件所在的页面被展示时执行: show()
            2. 组件所在的页面被隐藏时执行: hide()
            3. 组件所在的页面尺寸变化时执行: resize()
        小程序生命周期: 
            onLoad()
            onShow()
            onReady()
            onHide()
            onShow()
            onUnload()
10.服务器端
    Cookie？SessionStorage？LocalStorage？
        session 和 cookie 用于浏览器客户端与服务端数据交互, 通过会话的方式跟踪浏览器用户身份。
        cookie: 
            1. 一般由服务器生成, 可以设置失效时间, 如果是浏览器生成则默认浏览器关闭后失效。
            2. 与服务器端通信, 每次请求都放在 http 请求头中。
            3. 数据存储在内存中, 数据大小为4KB, 保存在类型为字符串。
            作用域: 
                1. 必须同源
                2. 可以是不同的tab页
                3. 不可以在不同的浏览器
                4. 要是同一个路径下或者子路径下
        session storage: 
            1. 失效时间, 当前页面或浏览器关闭
            作用域: 
                1. 必须同源
                2. 不可以在不同的tab页
                3. 不可以在不同的浏览器
        local storage: 
            1. 失效时间需要手动清除
            作用域: 
                1. 必须同源
                2. 可以在不同的tab页
                3. 可以在同一个浏览器的不同窗口中
                4. 不可以在不同的浏览器中访问
    Ajax的请求方式都有哪些？
        get理解为查询, delete就是删除, post就是新增, put就是更新数据
        ajax的缺点: 
            1. ajax不支持浏览器back按钮。
            2. 安全问题 AJAX暴露了与服务器交互的细节。
            3. 对搜索引擎的支持比较弱。
            4. 破坏了程序的异常机制。
            5. 不容易调试。
    说一下什么是跨域？如何解决跨域？
        解决跨域: 
            1. 通过jsonp跨域
                原理: 动态添加一个<script>标签, 而script标签的src属性是没有跨域的限制的。
                优点: 它不像XMLHttpRequest对象实现的Ajax请求那样受到同源策略的限制; 它的兼容性更好, 在更加古老的浏览器中都可以运行, 不需要XMLHttpRequest或ActiveX的支持; 并且在请求完毕后可以通过调用callback的方式回传结果。
                缺点: 它只支持GET请求而不支持POST等其它类型的HTTP请求; 它只支持跨域HTTP请求这种情况, 不能解决不同域的两个页面之间如何进行JavaScript调用的问题。
            2. document.domain + iframe跨域(仅限主域相同, 子域不同的跨域应用场景)
                实现原理: 两个页面都通过js强制设置document.domain为基础主域, 就实现了同域。
            3. location.hash + iframe
                实现原理: a域与b跨域相互通信, 通过中间页c来实现。 三个页面, 不同域之间利用iframe的location.hash传值, 相同域之间直接js访问来通信。
            4. window.name + iframe跨域
                window.name属性的独特之处: name值在不同的页面(甚至不同域名)加载后依旧存在, 并且可以支持非常长的 name 值(2MB)。
            5. postMessage跨域
                postMessage是HTML5 XMLHttpRequest Level 2中的API, 且是为数不多可以跨域操作的window属性之一, 它可用于解决以下方面的问题: 
                    1. 页面和其打开的新窗口的数据传递。
                    2. 多窗口之间消息传递。
                    3. 页面与嵌套的iframe消息传递。
                    4. 上面三个场景的跨域数据传递。
                        用法: postMessage(data,origin)方法接受两个参数。
                        data: html5规范支持任意基本类型或可复制的对象, 但部分浏览器只支持字符串, 所以传参时最好用JSON.stringify()序列化。
                        origin: 协议+主机+端口号, 也可以设置为"*", 表示可以传递给任意窗口, 如果要指定和当前窗口同源的话设置为"/"。
            6. 跨域资源共享(CORS)
                普通跨域请求: 只服务端设置Access-Control-Allow-Origin即可, 前端无须设置, 若要带cookie请求: 前后端都需要设置。
                需注意的是: 由于同源策略的限制, 所读取的cookie为跨域请求接口所在域的cookie, 而非当前页。
                目前, 所有浏览器都支持该功能(IE8+: IE8/9需要使用XDomainRequest对象来支持CORS), CORS也已经成为主流的跨域解决方案。
            7. nginx代理跨域
            8. nodejs中间件代理跨域
            9. WebSocket协议跨域
    说一下前端的SEO？
        1. 合理的title description keywords: 搜索对这三项的权重逐个减小title值强调重点即可; description把页面内容高度概括, 不可过分堆砌关键词; keywords列举出重要关键词。
        2. 语义化的HTML代码, 符合W3C规范: 语义化代码让搜索引擎容易理解网页。
        3. 重要内容HTML代码放在最前: 搜索引擎抓取HTML顺序是从上到下, 保证重要内容一定会被抓取。
        4. 重要内容不要用js输出: 爬虫不会执行js获取内容。
        5. 少用iframe: 搜索引擎不会抓取iframe中的内容。
        6. 非装饰性图片必须加alt。
        7. 提高网站速度: 网站速度是搜索引擎排序的一个重要指标。
        1. 减少HTTP请求次数
            尽量合并图片、CSS、JS。比如加载一个页面, 如果有5个css文件的话, 那么会发出5次http请求, 这样会让用户第一次访问你的页面的时候会长时间等待。而如果把这个5个文件合成一个的话, 就只需要发出一次http请求, 节省网络请求时间, 加快页面的加载。
        2. 使用CDN
            网站上静态资源即css、js全都使用cdn分发, 图片亦然。
        3. 避免空的src和href
            当link标签的href属性为空、script标签的src属性为空的时候, 浏览器渲染的时候会把当前页面的URL作为它们的属性值, 从而把页面的内容加载进来作为它们的值。所以要避免犯这样的疏忽。
        4. 为文件头指定Expires
            Exipres是用来设置文件的过期时间的, 一般对css、js、图片资源有效。 他可以使内容具有缓存性, 这样下回再访问同样的资源时就通过浏览器缓存区读取, 不需要再发出http请求。
        5. 使用gzip压缩内容
            gzip能够压缩任何一个文本类型的响应, 包括html, xml, json。大大缩小请求返回的数据量。
        6. 把CSS放到顶部
            网页上的资源加载时从上网下顺序加载的, 所以css放在页面的顶部能够优先渲染页面, 让用户感觉页面加载很快。
        7. 把JS放到底部
            加载js时会对后续的资源造成阻塞, 必须得等js加载完才去加载后续的文件 , 所以就把js放在页面底部最后加载。
        8. 避免使用CSS表达式
            举个css表达式的例子
                font-color: expression( (new Date()).getHours()%3 ? “#FFFFFF" : “#AAAAAA" );
                这个表达式会持续的在页面上计算样式, 影响页面的性能。并且css表达式只被IE支持。
        9. 将CSS和JS放到外部文件中
            目的是缓存文件, 可以参考原则4。 但有时候为了减少请求, 也会直接写到页面里, 需根据PV和IP的比例权衡。
        10. 权衡DNS查找次数
            减少主机名可以节省响应时间。但同时, 需要注意, 减少主机会减少页面中并行下载的数量。
            IE浏览器在同一时刻只能从同一域名下载两个文件。当在一个页面显示多张图片时, IE 用户的图片下载速度就会受到影响。所以新浪会搞N个二级域名来放图片。
        11. 精简CSS和JS
            这里就涉及到css和js的压缩了。比如下面的新浪的一个css文件, 把空格回车全部去掉, 减少文件的大小。现在的压缩工具有很多, 基本主流的前端构建工具都能进行css和js文件的压缩, 如grunt, glup等。
        12. 避免跳转
            有种现象会比较坑爹, 看起来没什么差别, 其实多次了一次页面跳转。比如当URL本该有斜杠(/)却被忽略掉时。例如, 当我们要访问 baidu.com 时, 实际上返回的是一个包含301代码的跳转, 它指向的是 baidu.com/(注意末尾的斜杠)。在nginx服务器可以使用rewrite；Apache服务器中可以使用Alias 或者 mod_rewrite或者the DirectorySlash来避免。
            另一种是不用域名之间的跳转,  比如访问 baidu.com/bbs 跳转到bbs.baidu.com/。那么可以通过使用Alias或者mod_rewirte建立CNAME(保存一个域名和另外一个域名之间关系的DNS记录)来替代。
        13. 删除重复的JS和CSS
            重复调用脚本, 除了增加额外的HTTP请求外, 多次运算也会浪费时间。在IE和Firefox中不管脚本是否可缓存, 它们都存在重复运算JavaScript的问题。
        14. 配置ETags
            它用来判断浏览器缓存里的元素是否和原来服务器上的一致。比last-modified date更具有弹性, 例如某个文件在1秒内修改了10次, Etag可以综合Inode(文件的索引节点(inode)数), MTime(修改时间)和Size来精准的进行判断, 避开UNIX记录MTime只能精确到秒的问题。 服务器集群使用, 可取后两个参数。使用ETags减少Web应用带宽和负载
        15. 可缓存的AJAX
            异步请求同样的造成用户等待, 所以使用ajax请求时, 要主动告诉浏览器如果该请求有缓存就去请求缓存内容。如下代码片段, cache:true就是显式的要求如果当前请求有缓存的话, 直接使用缓存
            $.ajax({      url : 'url',      dataType : "json",      cache: true,      success : function(son, status){                  }
        16. 使用GET来完成AJAX请求
            当使用XMLHttpRequest时, 浏览器中的POST方法是一个“两步走”的过程: 首先发送文件头, 然后才发送数据。因此使用GET获取数据时更加有意义。
        17. 减少DOM元素数量
            这是一门大学问, 这里可以引申出一堆优化的细节。想要具体研究的可以看后面推荐书籍。总之大原则减少DOM数量, 就会减少浏览器的解析负担。
        18. 避免404
            比如外链的css、js文件出现问题返回404时, 会破坏浏览器的并行加载。
        19. 减少Cookie的大小
            Cookie里面别塞那么多东西, 因为每个请求都得带着他跑。
        20. 使用无cookie的域
            比如CSS、js、图片等, 客户端请求静态文件的时候, 减少了 Cookie 的反复传输对主域名的影响。
        21. 不要使用滤镜
            IE独有属性AlphaImageLoader用于修正7.0以下版本中显示PNG图片的半透明效果。这个滤镜的问题在于浏览器加载图片时它会终止内容的呈现并且冻结浏览器。在每一个元素(不仅仅是图片)它都会运算一次, 增加了内存开支, 因此它的问题是多方面的。
            完全避免使用AlphaImageLoader的最好方法就是使用PNG8格式来代替, 这种格式能在IE中很好地工作。如果你确实需要使用AlphaImageLoader, 请使用下划线_filter又使之对IE7以上版本的用户无效。
        22. 不要在HTML中缩放图片
            比如你需要的图片尺寸是50* 50,  那就不用用一张500*500的大尺寸图片, 影响加载
        23. 缩小favicon.ico并缓存
    说一下前端的安全性问题？
        xss: 跨站脚本攻击(Cross Site Scripting)是最常见和基本的攻击 WEB 网站方法, 攻击者通过注入非法的 html 标签或者 javascript 代码, 从而当用户浏览该网页时, 控制用户浏览器。
            xss 主要分为三类: 
                1. DOM xss: DOM即文本对象模型, DOM通常代表在html、xhtml和xml中的对象, 使用DOM可以允许程序和脚本动态的访问和更新文档的内容、结构和样式。它不需要服务器解析响应的直接参与, 触发XSS靠的是浏览器端的DOM解析, 可以认为完全是客户端的事情。
                2. 反射型 xss: 反射型XSS也被称为非持久性XSS, 是现在最容易出现的一种XSS漏洞。发出请求时, XSS代码出现在URL中, 最后输入提交到服务器, 服务器解析后在响应内容中出现这段XSS代码, 最后浏览器解析执行。
                3. 存储型 xss: 存储型XSS又被称为持久性XSS, 它是最危险的一种跨站脚本, 相比反射型XSS和DOM型XSS具有更高的隐蔽性, 所以危害更大, 因为它不需要用户手动触发。 允许用户存储数据的web程序都可能存在存储型XSS漏洞, 当攻击者提交一段XSS代码后, 被服务器端接收并存储, 当所有浏览者访问某个页面时都会被XSS, 其中最典型的例子就是留言板。
            跨站脚本攻击可能会造成以下影响: 
                1. 利用虚假输入表单骗取用户个人信息。
                2. 利用脚本窃取用户的 Cookie 值, 被害者在不知情的情况下, 帮助攻击者发送恶意请求。
                3. 显示伪造的文章或图片。
            防御: 
                1. 输入检查, 一般是用于对于输入格式的检查, 例如: 邮箱, 电话号码, 用户名, 密码……等, 按照规定的格式输入。
                2. 不仅仅是前端负责, 后端也要做相同的过滤检查。
                3. 因为攻击者完全可以绕过正常的输入流程, 直接利用相关接口向服务器发送设置。
        csrf: 跨站点请求伪造(Cross-Site Request Forgeries), 也被称为 one-click attack 或者 session riding。冒充用户发起请求(在用户不知情的情况下),  完成一些违背用户意愿的事情(如修改用户信息, 删除评论等)。
            可能会造成以下影响: 
                1. 利用已通过认证的用户权限更新设定信息等。
                2. 利用已通过认证的用户权限购买商品。
                3. 利用已通过的用户权限在留言板上发表言论。
            与xss的区别: 
                1. 通常来说 CSRF 是由 XSS 实现的, CSRF 时常也被称为 XSRF(CSRF 实现的方式还可以是直接通过命令行发起请求等)。
                2. 本质上讲, XSS 是代码注入问题, CSRF 是 HTTP 问题。XSS 是内容没有过滤导致浏览器将攻击者的输入当代码执行。CSRF 则是因为浏览器在发送 HTTP 请求时候自动带上 cookie, 而一般网站的 session 都存在 cookie里面。
            案例: 
                1. 比如某网站的转账操作
                2. 受害者张三给李四转账100, 
                3. 通过对银行的网站发起请求 http://bank.example/transfer?accout=张三&a... , 
                4. 通常情况下, 该请求发出后, 服务器端会检查 session 是否合法, 并且张三已经登录成功, 
                5. 黑客王五可以自己给银行发送一个请求 http://bank.example/transfer?accout=张三&a... , 但是这个请求来自王五, 而不是张三, 他并不能通过安全认证。他需要张三的 session 。
                6. 王五自己做了一个网站, 放入如下代码 http://bank.example/transfer?accout=张三&a... , 
                7. 用各种方式诱使张三点击自己的网站。
                8. 张三登录了银行的网站没有退出, 访问了黑客王五的网站, 上述的 url 就会向银行发起请求。
                9. 如果session没有过期, 这时悲剧就发生了, 张三的账户里少了1000。
            防御: 
                1. 验证码；强制用户必须与应用进行交互, 才能完成最终请求。此种方式能很好的遏制 csrf, 但是用户体验比较差。
                2. 尽量使用 post , 限制 get 使用；上一个例子可见, get 太容易被拿来做 csrf 攻击, 但是 post 也并不是万无一失, 攻击者只需要构造一个form就可以。
                3. Referer check；请求来源限制, 此种方法成本最低, 但是并不能保证 100% 有效, 因为服务器并不是什么时候都能取到 Referer, 而且低版本的浏览器存在伪造 Referer 的风险。
                4. token；token 验证的 CSRF 防御机制是公认最合适的方案。
            整体思路如下: 
                1. 第一步: 后端随机产生一个 token, 把这个token 保存到 session 状态中；同时后端把这个token 交给前端页面；
                2. 第二步: 前端页面提交请求时, 把 token 加入到请求数据或者头信息中, 一起传给后端；
                3. 后端验证前端传来的 token 与 session 是否一致, 一致则合法, 否则是非法请求。
                4. 若网站同时存在 XSS 漏洞的时候, 这个方法也是空谈。
        Clickjacking:  点击劫持, 是指利用透明的按钮或连接做成陷阱, 覆盖在 Web 页面之上。然后诱使用户在不知情的情况下, 点击那个连接访问内容的一种攻击手段。这种行为又称为界面伪装(UI Redressing) 。
            大概有两种方式: 
                1. 攻击者使用一个透明 iframe, 覆盖在一个网页上, 然后诱使用户在该页面上进行操作, 此时用户将在不知情的情况下点击透明的 iframe 页面；
                2. 攻击者使用一张图片覆盖在网页, 遮挡网页原有的位置含义。
            一般步骤: 
                1. 黑客创建一个网页利用 iframe 包含目标网站。
                2. 隐藏目标网站, 使用户无法无法察觉到目标网站存在。
                3. 构造网页, 诱变用户点击特点按钮。
                4. 用户在不知情的情况下点击按钮, 触发执行恶意网页的命令。
            防御: 
                1. X-FRAME-OPTIONS HTTP 响应头是用来给浏览器指示允许一个页面可否在<frame>, <iframe> 或者 <object> 中展现的标记。网站可以使用此功能, 来确保自己网站内容没有被嵌到别人的网站中去, 也从而避免点击劫持的攻击。
                有三个值: 
                    1. DENY: 表示页面不允许在 frame 中展示, 即便是在相同域名的页面中嵌套也不允许。
                    2. SAMEORIGIN: 表示该页面可以在相同域名页面的 frame 中展示。
                    3. ALLOW-FROM url: 表示该页面可以在指定来源的 frame 中展示。
    如果让你做一个登录模块, 前端应该怎么做？你觉得后端应该怎么做？简述一下过程。
    说一下浏览器的协议？
        1. 地址栏输入url, 一系列的过程
        2. 200, 404, 500等代表啥
        3. http, https有啥区别
    WebSocket？
        客户端发送一次http websocket请求, 服务器响应请求, 双方建立持久连接, 并进行双向数据传输, 后面不进行HTTP连接, 而是使用TCP连接。
    TCP？UDP？TCP与UDP的区别？
        tcp: 
            三次握手, 用于传输比较小的数据
        udp: 
            不稳定用于传输音视频
        区别: 
            1. TCP面向连接(如打电话要先拨号建立连接);UDP是无连接的, 即发送数据之前不需要建立连接。
            2. TCP提供可靠的服务。也就是说, 通过TCP连接传送的数据, 无差错, 不丢失, 不重复, 且按序到达; UDP尽最大努力交付, 即不保证可靠交付。
            3. TCP面向字节流, 实际上是TCP把数据看成一连串无结构的字节流; UDP是面向报文的。
            UDP没有拥塞控制, 因此网络出现拥塞不会使源主机的发送速率降低(对实时应用很有用, 如IP电话, 实时视频会议等)。
            4. 每一条TCP连接只能是点到点的; UDP支持一对一, 一对多, 多对一和多对多的交互通信。
            5. TCP首部开销20字节;UDP的首部开销小, 只有8个字节。
            6. TCP的逻辑通信信道是全双工的可靠信道, UDP则是不可靠信道。
11.前端工具
    git跟svn有啥区别？
        1. git是分布式的, svn是集中式的
        2. git把内容按照元数据方式存储, 而非svn按文件: 因为git目录是处于个人机器上的一个版本克隆库, 它拥有中心版本库上所有的东西。例如: 标签、分支、版本记录等等。
        3. git分支和svn的分支不同: svn会发生分支遗漏情况, 而git可以在一个目录下快速的在几个分支间切换, 很容易发现未合并的分支, 简单而快捷的合并这些文件。
        4. git没有全局的一个版本号, 而svn有。
        5. git的内容完整性要优于svn: git的内容存储使用的是SHA-1哈希算法。这能确保代码内容的完整性, 确保在遇到磁盘故障和网络问题时降低对版本库的破坏。
    说一下webpack？说一下gulp？webpack跟gulp有啥区别？
        区别: 
            1. gulp是工具链、构建工具。可以配合各种插件做jps.压缩, css.压缩, less编译等, 可以替代手工实现自动化工作。
            2. webpack是文件打包工具, 可以把项目的各种jps.css.文件等打包合并成一个或多个文件, 主要用于模块化方案, 预编译模块的方案。
        gulp: 是一个自动化构建工具, 主要用来设定程序自动处理静态资源的工作。简单的说, gulp就是用来打包项目的。
            gulp.task('clean',function(){
                returngulp.src('./dist')
                .pipe(clean())
            })
            $ gulp clean
            gulp.src()
            gulp.dest()
            gulp.watch()

```
## 后端
```
1.你觉得mysql跟redis有啥区别？
    mysql: 是关系型数据库, 主要用于存放持久化数据, 将数据存储在硬盘中, 读取速度较慢。
    redis: 是NOSQL, 即非关系型数据库, 也是缓存数据库, 即将数据存储在缓存中, 缓存的读取速度快, 能够大大的提高运行效率, 但是保存时间有限。
    区别: 
    1.类型上
        从类型上来说, mysql是关系型数据库, redis是缓存数据库。
    2.作用上
        mysql用于持久化的存储数据到硬盘, 功能强大, 但是速度较慢。
        redis用于存储使用较为频繁的数据到缓存中, 读取速度快。
    3.需求上
        mysql和redis因为需求的不同, 一般都是配合使用。

```
