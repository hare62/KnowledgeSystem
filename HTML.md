#### **HTML：**

###### Doctype的作用？

> 文档声明，告诉浏览器以什么标准去渲染解析html

###### **标准模式和怪异模式的区别：**

> 标准模式的页面排版和JS运作模式都是浏览器支持的最高标准，而怪异模式是向后兼容，模拟老浏览器模式行为，防止页面无法正常工作



> **行内元素****/块级元素/空元素有哪些？**
>
> 行内元素:  a/img/span/b/strong/input/select/section
>
> 块级元素: div/p/table/ul/ol/li/h1-h6
>
> 空元素: br/hr/img/input/link/meta

###### **介绍一下你对浏览器内核的理解**

> 浏览器主要分为两个部分:渲染引擎和JS引擎
>
> 渲染引擎：主要负责获取页面内容和排版渲染页面
>
> JS引擎：解析和执行JS来实现页面的动态效果，以及交互内容
>
> 注意：js引擎和渲染引擎是互斥的，也就是说当前js引擎在运行的时候，渲染引擎不会工作，反之亦然，这也是为什么建议把通过script标签引入的脚本放到body后面，而不是body前面的原因。





**常用浏览器的内核有哪些？**
>chrome/safari-webkit
>Mozilla firefox-Gecko
>Opera-Presto
>IE-trident
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B321AE5635D4E27BF0EC851B50A20A2/4565](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B321AE5635D4E27BF0EC851B50A20A2/4565)
>
>  

**浏览器是怎么对****HTML5的离线储存资源进行管理和加载的？**

> · 在线的情况下，浏览器发现 html 标签有 manifest 属性，它会请求 manifest 文件
>
> · 如果是第一次访问app，那么浏览器就会根据 manifest 文件的内容下载相应的资源并且进行离线存储
>
> · 如果已经访问过app且资源已经离线存储了，浏览器会对比新的 manifest 文件与旧的 manifest 文件，如果文件没有发生改变，就不做任何操作。如果文件改变了，那么就会重新下载文件中的资源并进行离线存储
>
> · 离线的情况下，浏览器就直接使用离线存储的资源。
>
**描述一下****cookies/sessionStorage和localStorage的区别?**
>
> cookies是网站为了表示用户身份而储存在用户本地终端上的数据,Cookies的数据始终在同源的http请求中携带,会在浏览器和服务器中来回传递,大小不能4K(通常经过加密,所以不用担心账号被盗,同源策略[同源是指"协议+域名+端口"三者相同]可以防止XSS和CSRF攻击浏览器,XSS就是用过浏览器的cookies,截取用户数据,CSRF是模拟用户在网页上面的操作,完成数据请求.异步策略牵扯到了JSONP)
>
> sessionStorage和localStorage的数据都是在本地存储,不会把数据发给服务器,localStorage是关闭浏览器,数据还存在不会丢失,而sessionStorage是离开浏览器后,数据会自动删除.
>
**HTML5新特性有哪些？如何处理HTML5新标签的兼容性问题？如何区分HTML和HTML5？**
>
>HTML5新特性：
>
> 绘图方面：加入了canvas绘图和SVG绘图；
>
> 媒体方面： 加入了video和audio标签
>
> 语义化标签： 比如header、nav、footer、section ['sekʃ(ə)n]、article ['ɑrtɪkl]
>
> 本地离线存储： localStorage[ˈloʊkl] 和sessionStory两种本地离线缓存
>
> localStorage是长期储存数据,关闭浏览器后数据不会丢失
>
> sessionStorage是关闭浏览器后数据自动删除
>
> 表单控件:  calendar、date、time、email、url、search ;
>
> 以及一些新技术: webwoker / websocket (säkit)/ Geolocation(ˌjēōlōˈkāSHən)
>
> 如何区分HTML和HTML5: 通过Doctype声明/新增的结构元素/功能元素
>
>  
>
 **简述一下你对****HTML语义化的理解?**
>
> 用正确的标签做正确的事情，html语义化让页面的内容结构更加简单易懂，便于搜索引擎解析，便于阅读维护和理解
>
 **页面导入样式时****,使用link和@import有什么区别?**
>
> 1/link属于XHTML标签,除了加载CSS之外还能用于定义RSS,@import是CSS提供的,只能用于加载CSS
>
> 2/link加载的文件,在页面加载的时候,link文件会同时加载,而@import引入的CSS文件,是页面在加载完成后再加载的
>
> 3/@import有兼容性问题,IE5以下的浏览器是无法识别的,而link无兼容性问题
>
 **Iframe有哪些缺点?**
>
> Iframe会阻碍页面的onload事件
>
> 浏览器的搜索引擎一般读无法解读iframe页面,不利于SEO的搜索
>
> Iframe和主页面共享链接池,会影响页面的并行加载
>
> 使用js动态添加iframe  src属性,可以避免一三问题
>
**Label的作用是什么?怎么用?**
>label便签用可以让用户点击文字区域，自动聚焦到当前项的input框。
input设置id属性，label设置for属性，for属性的属性值为id属性值。
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5554CADFB47E42EB8ED164D33539DD34/4569](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5554CADFB47E42EB8ED164D33539DD34/4569)
>
>  
>
> label标签是定义表单控制间的关系,当用户点击label里面的文字时,浏览器会自动把光标转载表单控件上
>
**HTML5的form如何关闭自动完成功能?**
>
> 给不想要提示form或某个input设置autocomplete = off
>
**如何实现浏览器内多个标签之间的通信****?**
>
> ·  Websocket['sɒkɪt]/SharedWorker 都是可以将不同线程共享为一个线程,他们的数据也是共享的(没怎么用过,用法不太清楚)
>
> · LocalStorage 也可以实现浏览器多个标签页之间的通信
>A.js localStorage.setItem('namehare', name)
>B.js window.addEventListener('storage', function(event){    
>    alert(event.key + '=' + event.newValue)  
> })   
> · localStorage在另一个浏览器被添加/删除/修改时,会触发一个事件,我们可以通过对loacalStorage监听事件,控制他的值来进行信息通信

**页面可见性有哪些用途****?(visibility API)**
>
> 可以通过visibilityState检测当前页是否可见,以及打开网页的时间,可以 控制页面在被切换后,停止视频和音频的播放
>我们打开这个页面，然后再打开另一个页面，来回点击这两个页面，动画，视频，音频都可以在页面显示时打开，在页面隐藏时关闭。

**如何在页面上实现一个圆形的可点击区域****?**
>
> Border-radius
>
> 或者js实现,需要求一个点在不在圆上的算法,获取鼠标坐标等
>
**网页验证码是干嘛的****,解决了什么安全问题?**
>
> 区分用户是计算机还是人的公告全自动程序,可以防止恶意破解密码,刷票等
>
 **Title和h1的区别,b与strong的区别,i和em的区别?**
>
> title属性没有明确的标题,只是HTML语义化的一个标签,而h1则是层次明确的标题,h1标签里的文字,字体较大,并且会加粗
>
> b与strong都有加粗字体的作用,strong只是更加语义化,是加重语气的意思
>
> i和em,em是强化文本的内容,而所有浏览器对重要内容都是以斜体形式显示的,i则是表示,标签内文本为斜体
>
**<img>的title和alt有什么区别?**
>
> title是当鼠标划到图片元素时显示的图片描述
>
> alt是img的特有属性，是图片内容的等价描述，用于图片无法加载时显示、读屏器阅读图片。可提高图片可访问性，除了纯装饰性图片外都需要设置有意义的值，搜索引擎会重点分析。
>
**Web标准以及W3C标准是什么？**
> 标签闭合、标签小写、不乱嵌套，使用外链css和js、结构行为表现的分离
**xhtml和html有什么区别？**
>
> 功能上的差别：
>
> 主要是xhtml可兼各大浏览器、手机以及PDA，并且浏览器也能快速正确地编译网页
>
> 书写习惯的差别：
>
> xhtml元素必须被正确嵌套，闭合、区分大小写，文档必须拥有根元素
>
 **Canvas和Svg有什么区别?**
>
> svg绘制出来的每一个图形的元素都是独立的DOM节点,能够方便的绑定事件或用来修改。canvas输出的是一副画布
>
> svg输出的图形是矢量图形，后期可以修改参数来自由放大缩小，不会失真和锯齿。而canvas输出标量画布，就像一张图片一样，放大会失真或者锯齿
>
> **数据请求相关问题：**
>
> **http请求方式有哪些？**
>
> · HTTP1.0定义了三种请求方法： GET, POST 和 HEAD方法。
>
> · HTTP1.1新增了五种请求方法：OPTIONS, PUT, DELETE, TRACE 和 CONNECT 方法。
>
> **http的状态码有哪些？分别说下它们的含义**
>
> 1XX：信息状态码
>
> 2XX：成功状态码
>
> 3XX：重定向
>
> 4XX：客户端错误
>
> 5XX：服务器错误
>
> 常见状态码：
>
> 401  请求要求身份验证。对于需要登录的网页，服务器可能返回此响应
>
> 403  服务器已经理解请求，但是拒绝执行它。
>
> 404  请求失败
>
> 500 服务器遇到一个未曾预料的情况，导致无法完成对请求的处理
>
> 503  由于请示服务器维护或者过载，服务器当前无法处理请求
>
> **请描述一下****get与post的区别**
>
> W3schools上面的参考答案
>
> GET在浏览器回退时是无害的，而POST会再次提交请求
>
> GET产生的URL地址可被Bookmark，而POST不可以
>
> GET请求会被浏览器主动cache，而POST不会，除非手动设置
>
> GET请求只能进行url编码，而POST支持多种编码方式。
>
> GET请求参数会被完整的保留在浏览器历史记录中，而POST中的参数不会被保留
>
> GET请求在URL中传送的参数是有长度限制的，而POST没有
>
> 对参数的数据类型，GET只接受ASCII字符，而POST没有限制
>
> GET比POST更不安全，因为参数直接暴露在URL上，所以不能用来传递敏感信息
>
> GET参数通过URL传递，POST放在Request body中
>
> get与post都是http协议中的两种发送请求方式，由于http的层是TCP/IP，所以get与post的底层也是TCP/IP。而get产生一个TCP数据包，post产生两个TCP数据包。具体点来说就是：
>
> 对于Get方式的请求，浏览器会把http header和data一并发送出去，服务器响应200（返回数据）
>
> 对于Post方式的请求，浏览器先发送header，服务器响应100，浏览器再发送data，服务器响应200（返回数据）
>
> 这样看来Post需要两步，时间上消耗的要多一点。所以get比post更有效
>
> 但是：
>
> \1. get与post都有自己的语义，不能随便混用
>
> \2. 如果网络好的情况下，发一次包的时间和发两次包的时间差别基本可以无视。但是网络环境比较差的情况下，两次包的TCP在验证数据包完整性上，有很大的优点
>
> 并不是所有浏览器都会在POST中发送两次包，Firefox就只发送一次
>
 **http和https有何区别？如何灵活使用？**
>
> http协议传输的数据都是未加密的，也就是明文的，因此使用http协议传输隐私信息非常不安全。为了保证这些隐私数据能加密传输，于是网景公司设计了ssl(Secure Sockets Layer)协议用于对http协议传输的数据进行加密，从而就诞生了https。
>
> 简单来说，https协议是由ssl+http协议构建的可进行加密传输、身份认证的网络协议，要比http协议安全。
>
> 
>
> https和http的主要区别：
>
> 一、https协议需要到ca机构申请ssl证书(如沃通CA)，另外沃通CA还提供3年期的免费ssl证书，高级别的ssl证书需要一定费用。
>
> 二、http是超文本传输协议，信息是明文传输，https 则是具有安全性的ssl加密传输协议。
>
> 三、http和https使用的是完全不同的连接方式，用的端口也不一样，http是80端口，https是443端口。
>
> 四、http的连接很简单，是无状态的;https协议是由ssl+http协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。
>
> 五、如果要实现HTTPS那么可以淘宝Gworg获取SSL证书。
>
> >**跨域的几种方式**
>
> 首先了解一下同源策略：同源策略、SOP是一种约定，是浏览器最核心也会最基本的安全功能，如果缺少了同源侧罗，浏览器很容易受到XSS、CSRF等攻击。所谓同源是指“协议+端口+域名”三者相同，即便两个不通的域名指向同一个IP地址，也非同源。
>
> 怎样解决跨域问题？
>
> \1. 通过jsonp跨域
>
> 
**一次性插入****1000个div，如何优化插入的性能**
>
> 使用Fragment（document.createDocumentFragment( )）
>
> Documentfragments是DOM节点，它们不是DOM树的一部分。通常的用例是创建文档片段，将元素附加到文档片段，然后将文档片段附加到DOM树中。因为文档片段存在于内存中，并不在DOM树中，所以讲子元素插入到文档片段时不会引起页面回流。因为使用文档片段会带来更好的性能
>
> 先创建一个div，后续的复制这个元素，避免重复创建元素，再放到元素片段里面
>
> var divFragment = document.createDocumentFragment（）; 
>
> let div = document.createElement（“div”）; 
>
> for（var i = 0; i <1000; i ++）{ 
>
> divFragment.append（div.cloneNode（））
>
> } 
>
> document.body.appendChild（divFragment）;
>> **网页从输入网址到渲染完成经历了哪些过程？**
>
> 1）输入网址
>
> 2）发送到DNS服务器，并获取域名对应的web服务器对应的IP地址
>
> 3）与web服务器建立TCP连接
>
> 4）浏览器向web服务器发送http请求
>
> 5）web服务器响应请求，并返回一定url的数据（或错误信息，或重定向的新url地址）
>
> 6）浏览器下载web服务器返回的数据及解析html源文件
>
> 7）生成DOM树，解析css和js，渲染页面，直至显示完成
> 
**mouseover/mouseout与mouseenter/mouseleave的区别与联系**
>
> \1. mouseover/mouseout是标准事件，所有浏览器都支持；mouseenter/mouseleave是IE5.5引入的特有事件,后来被DOM3标准采纳，现代浏览器也支持
>
> mouseover/mouseout是冒泡事件;mouseenter/mouseleave不冒泡.需要为多个元素监听鼠标移入/移出事件时，推荐使用mouseover、mouseout托管，提高性能
>
> 
>**DOM元素的e的e.getAttribute(propName)和e.propName有什么区别和联系?**TODO
>
> e.getAttribute()是标准DOM操作文档元素属性的方法,具有通用性可在任意文档上使用，返回元素在源文件中设置的属性
>
> e.propName通常是在HTML文档中访问特定元素的特性，浏览器解析元素后生产对应对象，这些对象的特性会根据特定规则结合属性设置得到，对于没有对应特性的属性，只能使用getAttribute进行访问
>
> e.getAttribute（）返回值是源文件中设置的值，类型是字符串或者是null
>
> e.propName返回值可能是字符串、布尔值、对象、undefined等
>
> 大部分attribute与property是一一对应关系，修改其中一个会影响另外一个，如id、title等属性
>
> 一些布尔属性<input hidden/>的检测设置需要hasAttribute和removeAttribute来完成,或者设置对应的property
>
> 像<a href="../index.html">link</a>中的href属性，转换成property的时候需要通过转换得到完整的url
>
> 一些attribute和property不是一一对应，如：form控件中<input value="hello"/>对应的是defaultValue，修改或设置value property修改的是控件当前值，setattribute修改value属性不会改变value property
>
**offsetWidth/offsetHeight、clientWidth/clientHeight与scrollWidth/scrollHeight的区别？**
>
> offfsetWidth、offsetHeight返回值包含content+padding+border，效果与e.getBoundingClientRect（）相同
>
> clientWidth、clientHieight返回值值包含content+padding，如果有滚动条，也不包含滚动条
>
> scrollWidth、scrollHeight返回值包含content+padding+溢出内容的尺寸
>
**focus/blur与focusin/focusout的区别和联系**TODO
>
> \1. focus/blur不冒泡，focusin/focusout冒泡
>
> \2. focus/blur兼容性好，focusin、focusout在除fireFox外的浏览器下都保持良好兼容性，如需使用事件托管，可考虑FireFox下使用事件捕获
>
> elem.addEventListener(‘focus’,handler,true)
>
> \3. 可获得焦点的元素:
>
> window/链接被点击或键盘操作/表单控件被点击或键盘操作/设置tabindex属性的元素被点击或键盘操作
>
> \2. 
> 
 **document.write和innerHTML的区别?**
>
> document.write是直接写入到页面的内容流,如果在写之前没有调用document.open，浏览器会自动调用open。每次写完关闭后重新调用该函数，会导致页面被重写
>
> innerHTML则是DOM页面元素的一个属性，代表该元素的html内容，你可以精确到某一个具体的元素来进行更改。如果想修改document的内容，则需要修改document.documentElement.innerElement
>
> innerHTML将内容写入某个DOM节点，不会导致页面全部重绘，innerHTML很多情况下都优于document.write，其原因在于其允许更精准的控制要刷新页面的那个部分
>
> **createElement与createDocumentFragment****的区别****?**
>
> 共同点：
>
> \1. 添加子元素后返回值都是新添加的子元素
>
> \2. 都可以通过appendChild添加子元素，并且子元素必须是node类型，不能为文本
>
> \3. 若添加的子元素是文档中存在的元素，则通过appendChild在为其添加子元素时，会从文档中删除之存在的元素
>
> 不同点：
>
> \1. createElement创建的是元素节点，节点类型为1，createDocumentFragment创建的是文档碎片，节点类型是11
>
> \2. 通过createElement新建元素必须指定元素tagName，因为其可用innerHTML添加子元素。通过createDocumentFragment则不必
>
> \3. 通过createElement创建的元素是直接插入到文档中，而通过createDocumentFragment创建的元素插入到文档中的是他的子元素
**http和https区别**

```
http协议是明文报文，所以很容易被窃听，比如通过抓包工具就能获取http响应报文的全部内容。如何防止被窃听呢？
可以将通信加密，但是http是没有加密协议的，所以SSL协议就是就解决了这个问题。所以https = http + ssl

http协议的请求和响应不会确定对方身份。因此在通信过程中，就会造成伪装web服务器，伪装客户端，还有就是无法确定通信对方是否具备访问权限。也无法确定客户端的身份，服务端对于客户端的请求也是来者不拒，无法阻止海量请求，比如DOs攻击。TODO
想要解决这个问题，SSL协议也能解决这些问题，SSL使用一种被称为证书的，用于确认身份。即可解决不验证通信方的身份就可能遭遇伪装

通信过程中无法确认报文完整性，可能被中间人攻击并且篡改。让客户端和服务端之间的通信看上去是正常的。SSL提供加密处理、认证、摘要功能。
```