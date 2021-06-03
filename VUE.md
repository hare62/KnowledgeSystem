> **Vue**
>
> **什么是****MVVM?**
>
> MVVM分为Model、View、ViewModel三者。
>
> Model 代表数据模型，数据和业务逻辑都在Model层中定义；
>
> View 代表UI视图，负责数据的展示；
>
> ViewModel 负责监听 Model 中数据的改变并且控制视图的更新，处理用户交互操作；
>
> Model 和 View 并无直接关联，而是通过 ViewModel 来进行联系的，Model 和 ViewModel 之间有着双向数据绑定的联系。因此当 Model 中的数据改变时会触发 View 层的刷新，View 中由于用户交互操作而改变的数据也会在 Model 中同步。
>
> 这种模式实现了 Model 和 View 的数据自动同步，因此开发者只需要专注对数据的维护操作即可，而不需要自己操作 dom。
>
> **mvvm和mvc的区别？它和其他框架（JQuery）的区别是什么？哪些场景适合？**
>
> mvc和mvvm其实区别不大。都是一种设计思想，主要mvc中controller演变成mvvm中的ViewModel。mvvm主要解决了mvc中大量的DOM操作使页面渲染性能降低，加载速度变慢，影响用户体验
>
> 区别：vue数据驱动，通过数据来显示视图层而不是节点操作
>
> 场景：数据操作比较多的场景，更加便捷
>
> **Vue的优点是什么？**
>
> \1. 低耦合：视图View可以独立于Model变化和修改，一个ViewModel可以绑定到不同给的“view”上，当View变化的时候Model可以不变，当Model变化的时候View也可以不变。
>
> \2. 可重用性：你可以把一些视图逻辑放在ViewModel里面，让很多view重用这段视图逻辑
>
> \3. 独立开发：开发人员可以专注于业务逻辑和数据的开发（ViewModel），设计人员可以专注于页面设计
>
> \4. 可测试：界面素来是比较难测试的，而现在测试可以针对ViewModel来写
>
> **Vue组件之间的传值**
>
> -父组件与子组件传值
>
> 父组件通过标签上定义传值(:父组件名称=”子组件props的名称”)
>
> 子组件通过props的方式接受数据
>
> -子组件向父组件传递数据
>
> 子组件通过$emit方法传递参数给父组件
>
> **Vue-cli中怎么使用自定义组件，又遇到过哪些问题吗?**
>
> 1) 在components文件中创建组件.vue文件.是script中export default{}
>
> 2) 在调用的页面中使用import XXX from 路径
>
> 3) 在调用的组建components属性中注册组件，注意大小写（文档不接受-连字符，可以使用驼峰命名）
>
> **Vue如何实现按需加载配合webpack设置**
>
> webpack中提供了require ensure（）来实现按需加载。以前引入路由是通过import这样的方式引入，现在改为 const定义的方式他引入。
>
> 不进行页面按需加载引入方式：import home from ‘../XXX’
>
> 进行页面按需加载的引入方式：const home = ‘../XXX’
>
> **v-show和v-if指令的共同点和不同点**
>
> v-show指令是通过修改元素的display的CSS属性让其显示或隐藏
>
> v-if指令是直接销毁和重建DOM节点，达到让元素显示和隐藏的效果
>
> **如何让****CSS只在当前组件中起作用**
>
> 在当前文档中使用style标签，并添加scope属性
>
> **<keep-alive></keep-alive>的作用是什么？**
>
> keep-alive标签包裹动态组件时，会缓存不活动的组件实例，主要用于保留组件状态或避免重新渲染
>
> **Vue中引入组件的步骤**
>
> 1) 采用 ES6的import...from...语法或CommonJS的require()方法引入组件
>
> 2) 对组件进行注册
>
> *// 注册*
>
> Vue.component('my-component', {
>
> template: '<div>A custom component!</div>'
>
> })
>
> 3) 使用组件<my-component></my-component>
>
> **指令****v-el的作用是什么?**
>
> 提供一个在页面上已存在的DOM元素作为Vue实例的挂载目标，可以是CSS选择器，也可以是一个HTMLElement实例
>
> **在****Vue中使用插件的步骤**
>
> 采用ES6的import...from...语法或CommonJS的require()方法引入插件
>
> 使用全局方法Vue.use(plugin)使用插件，可以传图一个选项对象Vue,use(MyPlugin,{someOption:true })
>
> **active-class是哪个组件的属性？**
>
> vue-router模块的router-link组件
>
> **说出至少****4中vue当中的指令和它的用法？**
>
> v-if：判断是否为真，然后重组、销毁DOM节点
>
> v-for：数据循环
>
> v-bind：class 绑定一个属性
>
> v-model：实现双向绑定
>
> v-on：添加事件
>
> v-else：配合v-if使用
>
> **vue-loader是什么？使用它的用途有哪些？**
>
> 解析：vue文件的一个加载器
>
> 用途：js可以写es6、style样式可以scss、template可以加等
>
> **scss是什么？在vue-cli中安装使用步骤？有几大特性？**
>
> scss是css的预编译。
>
> **使用步骤：**
>
> \1. 先安装css-loader、node-loader、scss-loader等加载器模块
>
> \2. 在build目录找到webpack.base.config.js，在那个extends属性中加一个拓展scss
>
> \3. 在同一个文件，配置一个module属性
>
> \4. 在组件的style标签上添加lang属性，lang=“scss”
>
> **特性：**
>
> 可以使用变量（$变量名=值）;
>
> 可以用混合器
>
> 可以嵌套
>
> **为什么使用****key?**
>
> 当有相同标签名的元素切换时，需要通过key特性设置唯一的值来标记已让vue区分它们，否则vue为了效率只会替换相同标签内部的内容。
>
> **为什么避免****v-if和v-for用在一起？**
>
> 当vue处理指令时，v-for比v-if具有更高的优先级，通过v-if移动到容器元素，不会再重复遍历列表中的每个值，取而代之的事，我们只检查它一次，且不会再v-if为否的时候运行v-for。
>
> **VNode是什么？虚拟DOM是什么？**
>
> Vue在羽绒棉上渲染的节点，及其子节点成为“虚拟节”，简写为“VNode”。“虚拟DOM”是由Vue组件树简历起来的整个VNode树的称呼
>
> **MINI UI是什么？怎么使用？说出至少三个组件的使用方法？**
>
> 基于vue前端的组件库。使用npm安装，然后import样式和js；
>
> vue.use(miniUi)全局引入。在单个组件局部引入；
>
> import {Toast} form ‘mini-ui’；
>
> 组件一:  Toast（‘登录成功’）
>
> 组件二： mint-header；
>
> 组件三：mint-swiper
>
> **自定义指定****(v-check/v-focus)的方法有哪些？有哪些钩子函数？还有哪些钩子函数参数？**
>
> 全局定义指令：在vue对象的directive方法里面有两个参数，一个是指令名称，另外一个是函数。组件内定义指令：directives钩子函数：bind（绑定事件触发）、inserted（节点插入的时候触发）、updata（组件内相关更新）
>
> 钩子函数的参数：el、binding
>
> 
>
> **Vue封装组件的过程**
>
> 首先，使用Vue.extend( )创建一个组件
>
> 再使用Vue.component( )方法注册组件
>
> 接着,如果子组件需要数据，可以在props中接受定义
>
> 最后，子组件修改好数据后，想把数据传递给父组件，可以使用emit（）方法
>
> **Vue的****响应式原理是什么？**
>
> vue.js是才用数据劫持介个发布-订阅者模式的方法，通过object.defineProperty()来劫持各个属性的setter和getter，在数据变动时发布消息给订阅者，触发相应的监听回调。
>
> **简单描述每个周期具体适合哪些场景**
>
> 生命周期钩子的一些使用方法：
>
> beforecreate：可以在这加个loading事件，在加载实例时触发
>
> created：初始化完成时的时间写在这里，如在这结束loading事件，异步请求也适宜在这里调用
>
> mounted：挂载元素，获取到DOM节点
>
> updated：如果对数据统一处理，在这里写上相应函数
>
> beforeDestroy：可以做一个确认停止事件的确认框
>
> nextTick：更新数据后立即操作DOM
>
> **打包****Vue项目命令是什么?**
>
> npm run build
>
> **生命周期相关面试题**
>
> 生命总共分为8个阶段创建前/后、载入前/后、更新前/后、销毁前/后
>
> **创建前****/后** :
>
> 在beforeCreate阶段，vue实例的挂载元素el和数据对象data都为undefined，还未初始化。
>
> 在created阶段，vue实例的数据data有了，el还没有
>
> **载入前****/后**：
>
> 在beforeMount阶段，vue实例的$el和data都初始化了,单还没有挂载之前都是虚拟的demo阶段,data.message还未替换.
>
> 在mounted阶段,vue实例挂载完后,data.message成功渲染.
>
> **更新前****/后**：当data变化时,户触发beforeUpdate和update方法。
>
> **销毁前****/后**：
>
> 在执行destroy方法后，对data的改变不会再触发周期函数，说明此时vue实例已经结束了事件监听以及和dom的绑定，但是dom结构依然存在。
>
> **什么是****vue生命周期？**
>
> vue实例从创建到销毁的过程，就是生命周期。也就是从开始创建、初始化数据、编译模板、挂载DOM→渲染、更新→渲染、卸载等一系列过程，我们称这是Vue的生命周期。
>
> **vue生命周期的作用是什么？**
>
> 生命周期中有多个事件钩子，让我们在控制整个Vue实例的过程中更容易形成好的逻辑
>
> **vue生命周期总共有几个阶段？**
>
> 总共可以分8个阶段：创建前/后、载入前/后、更新前/后、销毁前/后
>
> 第一次页面加载会触发哪几个钩子?
>
> 第一次页面加载时会触发beforeCreate、created、beforeMount、mounted这几个钩子
>
> **请列举出****3个Vue常用的声明周期钩子函数**
>
> created：实例已经创建完成之后调用，在这一步，实例已经完成数据观测、属性和方法的运算，watch、event事件回调，然而，挂载阶段还没有开始，$el属性目前还不可见
>
> mounted：el被新创建的vm.$el替换，并挂载到实例上去之后调用该钩子,如果root实例挂在了一个文档内元素，当mounted被调用时vm.$el也在文档内。
>
> activated：keep-alive组件激活时调用
>
> **DOM渲染在那个周期中已完成？**
>
> DOM渲染在mounted中就已经完成了
>
> **Vue-router**
>
> **路由之间的跳转****:**
>
> 声明式（标签跳转）：<router-view>标签用于展示路由组件，DOM节点中使用v-link进行跳转，或使用router-link标签
>
> 编程式（js跳转）
>
> **怎么定义****vue-router的动态路由以及如何获取传过来的动态参数？**
>
> 在router目录下的index.js文件中，对path属性加上/：id
>
> 使用router对象的params id
>
> **Vue中,如何用watch去监听router变化**
>
> 当路由发生变化的时候，在watch中写具体的业务逻辑
>
> let vm = new Vue({
>
> el:"#app",
>
> data:{},
>
> router,
>
> watch:{
>
> $router(to,from){
>
> console.log(to.path);
>
> }
>
> }
>
> })
>
> 
>
> **vue-router有哪几种导航钩子？以及它的参数？**
>
> 三种，一是全局导航钩子：router.beforeEach(to,from,next)，作用：跳转前进行判断拦截。
>
> 第二种：组件内的钩子
>
> 第三种：单独路由独享组件
>
> beforeRouteEnter、afterEnter、beforeRouterUpdate、beforeRouteLeave
>
> 参数：有to（去的那个路由）、**from**（离开的路由）、**next**（一定要用这个函数才能去到下一个路由，如果不用就拦截）最常用就这几种
>
> **Vuex:**
>
> Vuex是一个专门为vue.js应用设计的状态管理架构，统一管理和维护各个Vue组件的可变化状态（可以理解为Vue组件中的那些data）
>
> **Vuex的五大属性:**
>
> Vue有五个核心概念：state、getters、mutations、actions、modules
>
> state  => 基本数据
>
> getters  =>  从基本数据派生的数据
>
> mutations  => 提交更改数据的方法，同步!
>
> actions  => 像一个装饰器，包裹mutations，使之可以异步
>
> modules =>  模块化Vuex
>
> **不用****Vuex会带来什么问题?**
>
> 1) 可维性会下降，想修改数据要维护三个地方
>
> 2) 可读性会下降，因为一个组件里的数据，根本就看不出来是从哪来的；
>
> 3) 增加耦合，大量的上传派发，会让耦合性大大增加。而Vue用Component就是为了减少耦合
>
> 
>
> 
>
