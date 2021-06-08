**React**
>
**react生命周期函数：**
>
> 这个问题考察组件的声明周期：
>
> 一．初始化阶段
>
> construct
>
> componentWillMount:组件即将被装载、渲染到页面上
>
> render：组件在这里生成虚拟的DOM节点
>
> componentDidMount：组件真正在被装载之后
>
> 二．运行中状态
>
> componentWillReceiverProps：组件将要接收到属性的时候调用
>
> shouldComponentUpdate：组件接受到新属性或者新状态的时候（可以返回false，接受数据后不更新，组织render调用，后面的函数不会被继续执行了）
>
> componentWillUpdate：组件即将更新不能修改属性和状态
>
> render：组件重新描绘
>
>componentDidMount：组件真正在被装载之后
>
> 三．销毁阶段
>
> componentWillUnmount：组件即将销毁
> 
>
**react性能优化是哪个周期函数？**
>
> 这个生命周期函数可以用来判断是否需要执行后面的生命周期函数比如(componentWillUpdate,render,componentDidUpdate)
> 避免了无效render，可以避免无效的重新渲染dom。便可以提高性能。
>
**在生命周期中的哪一步你应该发起****AJAX请求？**
>
> 我们应当将AJAX请求放到componentDidMount函数中执行，主要原因有下：
>
> 页面的dom已经挂在完毕，可以请求数据重新render到页面上。在这方法中调用setState方法，会触发重渲染。所以，官方设计这个方法就是用来加载外部数据用的，或处理其他的副作用代码。
> componentWillMount这个生命周期的dom还没有挂在到页面所以这个生命周期函数去请求数据然后想要去dom上渲染会找不到dom。
>
> 如果我们将AJAX请求放置在生命周期的其他函数中，我们并不能保证请求仅在组件挂载完毕后才会要求响应。如果我们的数据请求在组件挂载之前就完成，并且调用了setState函数将数据添加到组件状态中，对于为挂载的组件则会报错。而在componentDidMount函数中进行AJAX请求则能有效避免这个问题。
>
**调用****setState之后发生了什么？**
>
> 在调用setState函数之后，React会将传入的参数对象与组件当前的状态合并，然后触发所谓的调和过程（Reconciliation）。经过调和过程，React会以相对高效的方法根据新的状态构建React元素树并且着手重新渲染整个UI界面。React得到元素树之后，React会自动计算出新的树与老树的节点差异，然后根据差异对界面进行最小化重渲染。在差异计算算法中，React能够相对精确的知道哪些位置发生了改变以及应该如何改变，这就保证了按需更新，而不是全部重新渲染。
>
**传入****setState函数的第二个参数的作用是什么?**
>
> 该函数会在setState函数调用完成并且组件开始重新渲染的时候被调用，我们可以用该函数来监听渲染是否完成：
>
```
this.setState(
{
username:"tylermcginnis33",
() => .console.log('setState has finished and the component has re-rendered');
}
)
```
>
> **createElement与cloneElement的区别是什么？**
>
> createElement函数是JSX编译之后使用的创建React Element的函数，而cloneElement则是用于复制某个元素并传入新的Props。
>
> **为什么我们需要使用****React提供的Children API而不是JS的map？**
```
因为this.props.children的值有三种可能：

如果当前组件没有子节点，它的值就是undefined

如果当前组件只有一个子节点，它的值就是我object

如果当前组件有多个子节点，它的值就是array

当this.props.children的值不是数组时，使用js的map会报错，React提供了工具方法React.Children来处理this.props.children,它已经将this.props.children的所有情况考虑在内了。
```

>
> **React中的Element与Component的区别是？**
>
> React Element是描述屏幕上所见内容的数据结构，是对于UI的对象表述，典型的React Element就是利用JSX构建的声明式代码片然后被转化为createElement的调用组合。而React Component则是可以接收参数输入并且返回某个React Element的函数或者类。
>
> 新的react包含了：React.createElement、.createClass 、.Component 、
>
> .propTypes、 .children以及其他元素和组件类。这些都是你需要构建组件时的助手。
>
> 而react-dom包含了ReactDOM.render、.unmountComponentAtNode0和
>
> .findDOMNode 在react-dom/server， 有ReactDOMServer.renderToString和
>
> .renderToStaticMarkup服务器端渲染支持。
>
**在什么情况下你会优先选择使用****class Component而不是functional Component？**
>
> 在组件主要包含内部状态或者使用到生命周期函数的时候使用class Component，否则使用函数式组件，否则使用函数式组件。
>
> **React中refs的作用是什么？**
>
> refs是React提供给我们的安全访问DOM元素或者某个组件实例的句柄。我们可以为元素添加ref属性然后在回调函数中接受该元素在DOM树中的句柄，该值会作为回调函数的第一个参数返回：
>
> class CustomForm extends Component{
>
> handleSubmit = () => {
>
> console.log("Input Value",this.input.value)
>
> }
>
> render(){
>
> return(
>
> <form onSubmit = {this.handleSubmit}>
>
> <input type="text" ref={(input) => this.input = input}/>
>
> <button type="submit">Submit</button>
>
> </form>
>
> )
>
> }
>
> }
>
> 上述代码中的input域包含了一个ref属性，该属性声明的回调函数会接收input对应的DOM元素，我们将其绑定到this指针以便在其他的类函数中使用。另外值得一提的是，refs并不是类组件的专属，函数式组件同样能够利用闭包暂存其值：
>
> function CustomFrom({handleSubmit}){
>
> let inputElement
>
> return (
>
> <form onSubmit={()=>handleSubmit(inputElement.value)}>
>
> <input type='text' ref={(input)=>inputElement=input}/>
>
> <button type='submit'>Submit</button> 
>
> </form>
>
> )
>
> }
>
**React中keys的作用是什么？**
>
```
 Keys是React用于追踪哪些列表中元素被修改、被添加或者被移除的辅助标识。

 render(){
 return(
        <ul>
          {this.state.todoItems.map(({task,uid})=>{
          return <li key={uid}>{task}</li>
        })}
        </ul>
    )
}
 ```
>
> 在开发过程中，我们需要保证某个元素的key在其统计元素中具有唯一性。在React Diff算法中React会借助元素的Key值来判断该元素是新近创建的还是被移动而来的元素，从而减少不必要的元素重渲染。此外React还需要借助key值来判断元素与本地状态的关联关系，因此我们绝不可忽视转换函数中key的重要性。
>
> **diff算法？**
>
```
把树结构按照层级分解，值比较同级元素。
给列表结构的每个单元添加唯一的key属性，方便比较
React只会匹配项通class的component（这里面的class指的是组件的名称）
合并操作，调用component的setState方法的时候，React将其标记为dirty到每一个事件循环结束，React检查所有标记dirt component重新绘制选择性子树渲染，开发人员可以重写shouldComponentUpdate提高diff的性能
```
>
> 参考链接：https：//segmentfault.com/a/1190000000606216
>
 **React性能优化方案？**
>
 ```
 \1. 重写shouldComponentUpdate来避免不必要的dom操作

 \2. 使用production版本的react.js

 \3. 使用key来帮助React识别列表中所有子组件的最小变化

 参考链接 : https://segmentfault.com/a/1190000006254212﻿
 ```

**为什么虚拟****DOM会提高性能？**
>
```
虚拟dom相当于在js和真实dom中间加了一个缓存，利用dom diff算法避免了没有必要的dom操作，从而提高性能。
具体实现步骤如下：
用js对象结构表示DOM数的结构，然后这个树构造一个真正的DOM树，插到文档中
当状态变更的时候，重新构造一颗树的对象树。然后用新的树和旧的树进行比较，记录两棵树的差异。
把2所记录的差异应用到步骤1所构建的真正的DOM数上，视图就更新了。
```
>
> **简述****flux思想**
>
> flux的最大特点，就是数据的“单向流动”
>
> \1. 用户访问View
>
> \2. View发出用户的Action
>
> \3. Dispatcher收到Action，要求Store进行相应的更新
>
> \4. Store更新后，发出一个“change”事件
>
> \5. View收到“change”事件后，更新页面
>
> 参考链接：http://www.ruanyifeng.com/blog/2016/01/flux.html﻿
>
> **React项目用过什么脚手架？Mern？Yeoman？**
>
> Mern：Mern是脚手架的工具，它可以很容易的使用Mongo，Express，React and NodeJS生成同构JS应用。它最大限度的减少安装时间，并得到您使用的成熟技术来加速开发。
>
> **React组件的划分-业务组件和技术组件？**
>
> 根据组件的职责，通常把组件分为UI组件和容器组件
>
> UI组件负责UI的呈现，容器组件负责管理数据和逻辑
>
> 两者通过React-redux提供connect方法联系起来。
>
> 具体使用方法参考地址：
>
> ﻿http://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_three_react-redux.html﻿
>
> 
>
> **react高阶组件是什么？有什么作用？**
>
> 高阶组件就是接受一个组件作为参数，在函数中对组件做一系列的处理，随后返回一个新的组件作为返回值。
>
> 作用：1、代码复用，逻辑抽象，抽离底层准备（bootstrap）代码
>
> 2、渲染劫持
>
> 3、State 抽象和更改
>
> 4、Props 更改
>
> **PureComponent****（纯组件）的重要性和使用场景**
>
> PureComponent改变了生命周期方法shouldComponentUpdate，并且它会自动检查组件是否需要重新渲染。这时，只有PureComponent检测到state或者props发生变化时，PureComponent才会调用render方法，PureComponent仅仅是浅比较(shadow comparison)，所以改变组件内部的props或者state，它将不会发挥作用。
>
> 使用PureComponent的最佳情况就是展示组件，它既没有子组件，也没有依赖应用的全局状态。
>
> 
>
> **React-router:**
>
> **react-router的原理：**
>
> react-router就是控制不同的url渲染不同的组件。react-router在history库的基础上，实现了URL与UI的同步。
>
> **原理：**DOM渲染完成之后，给window添加onhashchange事件监听页面hash的变化，并且在state属性中添加了route属性，代表当前页面的路由。
>
> **具体步骤：**
>
> 当点击链接，页面hash改变时，触发绑定在 window 上的 onhashchange 事件；
>
> 在 onhashchange 事件中改变组件的 state中的 route 属性，react组件的state属性改变时，自动重新渲染页面；
>
> 页面随着 state 中的route属性改变，自动根据不同的hash给Child变量赋值不同的组件，进行渲染。
>
> 
>
> **用过****React-router吗？router 3.X和router 4.X区别在哪？**
>
> router 3.X
>
> l 路由集中在一处；
>
> l 布局和页面的层叠由层叠的 <Route> 组件控制；
>
> l 布局和页面组件是路由的一部分；
>
> React Router 4
>
> l 不再提倡中心化路由,路由不集中在一起。取之的是路由存在于布局和 UI 之间。
>
> l 不需要再在嵌套组件中使用 {props.children}
>
> l location.query属性没有了，现在通过 'query-string' 模块进行转换获取
>
> import queryString from  'query-string'
>
> let query=this.query=queryString.parse(location.search);
>
> 
>
> **react-router里hashHistory 和 browserHistory 的区别**
>
> react-router提供了三种方式来实现路由，并没有默认的路由，需要在声明路由的时候，显式指定所使用的路由。
>
> browserHistory（官方推荐)）、hashHistory、createMemoryHistory
>
> 区别：使用hashHistory,浏览器的url是这样的：/#/user/liuna?_k=adseis
>
> 使用browserHistory,浏览器的url是这样的：/user/liuna
>
> 这样看起来当然是browerHistory更好一些，但是它需要server端支持。
>
> 使用hashHistory时，因为有 # 的存在，浏览器不会发送request,react-router 自己根据 url 去 render 相应的模块。
>
> 使用browserHistory时，从 / 到 /user/liuna, 浏览器会向server发送request，所以server要做特殊请求，比如用的 express 的话，你需要 handle所有的路由 app.get('*', (req, res) => { ... })，使用了 nginx 的话，nginx也要做相应的配置。
>
> ​    如果只是静态页面，就不需要用browserHistory,直接hashHistory就好了。
>
> 
>
> **redux：**
>
> **redux中间件:**
>
> 中间件提供第三方插件的模式，自定义拦截action->reducer的过程.变为action->middlewares->reducer。这种机制让我们改变数据流，实现如异步action，action过滤，日志输出，异常报告等功能
>
> **redux常见的中间件：**
>
> redux-logger：提供日志输出
>
> redux-thunk：处理异步操作
>
> redux-promise：处理异步操作，sctionCreator的返回值是promise
>
> **redux有什么缺点？**
>
> \1. 一个组件所需要的数据，必须由父组件传过来，而不能像flux中直接从store取
>
> \2. 当一个组件相关数据更新时，即使父组件不需要用到这个组件，父组件还是会重新render，可能会有效率影响，或者需要写复杂的shouldComponentUpdate进行判断。
>
> 
>
> **redux三大原则：**
>
> 1、单一数据源：整个应用的 [**state**](https://note.youdao.com/newEditor/bulb.html#state) 被储存在一棵 object tree 中，并且这个 object tree 只存在于唯一一个 [**store**](https://note.youdao.com/newEditor/bulb.html#store) 中。
>
> 2、State 是只读的： 唯一改变 state 的方法就是触发 [**action**](https://note.youdao.com/newEditor/bulb.html#action)，action 是一个用于描述已发生事件的普通对象。这样确保了视图和网络请求都不能直接修改 state，相反它们只能表达想要修改的意图。
>
> 3、使用纯函数来执行修改： 为了描述 action 如何改变 state tree ，你需要编写 [reducers](https://note.youdao.com/newEditor/bulb.html#reducer)。Reducer 只是一些纯函数，它接收先前的 state 和 action，并返回新的 state。
>
> **React Native：**
>
> **React Native相对于原生的IOS和Android有哪些优势？**
>
> \1. 性能媲美原生APP
>
> \2. 使用JavaScript编码，只要学习这一种语言
>
> \3. 绝大部分代码安卓与IOS都能共用
>
> \4. 组件化开发，代码重用性高
>
> \5. 跟编写网页一般，修改代码后即可自动刷新，不需要慢慢编译，节省了很多编译等待时间
>
> \6. 支持APP热更新，更新无需重新安装App
>
> **缺点：**内存占用相对较高，版本不稳定，一直在更新。
>
> **React Native组件的生命周期:**
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/340485581DAA46E3B5E65BC99BE43CA2/4581](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/340485581DAA46E3B5E65BC99BE43CA2/4581)
>
> 
>
> **1.** **当页面第一次加载时，会依次调用：**
>
> constructor（）
>
> componentWillMount（）: 这个函数调用时机是在组件创建，并初始化了状态之后，在第一次绘制render（）之前，可以在这里做一些业务初始化操作，也可以设置组件状态。这个函数在整个生命周期中只被调用一次。
>
> render（）：组件渲染
>
> componentDidMount（）：虚拟DOM已经构建完成，你可以在这个函数开始获取其中的元素或者子组件了。需要注意的是，RN框架是先调用了子组件的componentDidMount（），然后调用父组件的函数。从这个函数开始，就尅和JS其他框架交互了，例如设置计时器setTimeout或者setInterval,或者发起网络请求.这个函数也是只被调用一次.这个函数之后,就进入了稳定运行状态,等待事件触发.
>
> **2.** **页面状态****state更改时：**

react与传统前端的对比
```
传统前端更改试图需要操作dom，会大量去操作dom这样。后来发现，将前端工作抽象出来，其实视图的改变对应着数据的改变，那么如果前端能只记录数据的变化，就可以将视图对应改变的话，那么前端就省了很多操作dom的工作。我们把数据变化通知到视图层变化交给react去做。于是react就诞生了。react就是一个UI库。

react不是直接操作dom而是映射出虚拟dom反应真实的dom，react用diff算法将新的虚拟dom和旧的虚拟dom比对，计算出变化的部分，再将变化的dom作用真实的dom上，把修改的虚拟dom重新渲染，极大的降低了前端亲自操作dom的工作，同时，得益于diff算法，性能上跟直接操作dom几乎一致。
```
**JSX**
```
jsx不是真的html,是通过react.createElement()的一种语法糖，返回的是ReactElement。这个可以加react的虚拟dom。
```