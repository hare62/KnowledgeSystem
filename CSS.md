> ****CSS:****
>
> **☆浏览器盒模型?**
>
> 盒模型分为两种: IE盒模型和W3C盒模型
>
> W3C标准盒模型: 宽度 = 内容宽度  宽度/padding/border/margin都是单独分开的
>
> IE盒模型: 经常用的是IE盒模型 宽度 = 内容宽度+padding+border 是一起的
>
**☆清除浮动的方式**
>
> \1. 在子元素并级后面添加一个新元素，添加clear：both属性
>
> 优点：通俗易懂，容易掌握
>
> 缺点：添加无意义空标签，不方便后期维护


> \2. 给父元素添加overflow:hidden
>
> 优点：代码较少，简单方便
>
> 缺点：不能配合定位使用


> \3. ：after方法（作用于浮动元素的父元素）
>
> .clearfix:after{
>
> content:"";
>
> display: block;
>
> height:0;
>
> clear:both;
>
> visibility:hidden;
>
> }
>
> /* 为兼容IE6,IE7，因为ie6,ie7不能用after伪类 */
>
> .clearfix{
>
> zoom:1;
>
> }
>
> 优点：结构和语义化完全正确
>
> 缺点：复用方式不当，会造成代码量增加


 **CSS选择器有哪些?哪些属性可以继承?**
>
> 选择器: ID选择器 (#ID)
>
> Class选择器 (.class名)
>
> 标签选择器 (标签)
>
> 通配符 (*)
>
> 相邻选择器 (div+p)
>
> 子选择器 (div>p)
>
> 后代选择器 (div p)
>
> 多个选择器 (div,p,a,ul)
>
> 伪类选择器 (a:hover)
>
> 拓展内容: 
>
**伪类选择器和伪元素的区别****:**
>
> 伪类用于向某些选择器添加特殊效果 (单冒号)
>
> 伪元素用于将某个特殊的东西添加到某些元素的前后 (双冒号)


> 伪类:
>
>
> |      |                                                              |
> | ---- | ------------------------------------------------------------ |
> |      | ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/60F0BBAA2D5A4DBDB16F312BF79DAC6A/4560](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/60F0BBAA2D5A4DBDB16F312BF79DAC6A/4560) |



> 伪元素:
>
> |      |                                                              |
> | ---- | ------------------------------------------------------------ |
> |      | ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/D13DBCCCCC1D45AE9A293F7DE41CA391/4559](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/D13DBCCCCC1D45AE9A293F7DE41CA391/4559) |
>
> 
>
> 
>
**::after/:after与::before/:before的区别?**
>
> :before在元素之前添加效果/:after是在元素之后添加效果
>
> :after/:before是CSS2提出的,兼容IE8
>
> ::after/::before是CSS3为了区分伪类和伪元素的做出的差别,为了避免兼容性问题,习惯性的还是写:after/:before;
>
> 
>
> 可继承样式: font-size/fon-family/color  [ul/li/ol/dl/dd/dt]
>
> 不可继承样式:width/height/margin/padding/border
>
 **CSS样式优先级计算法:**
>
> 三条标准:
>
> 1/就近原则,后加样式优于前面的样式
>
> 2/内嵌样式>内联样式>外联样式
>
> 3/!Important 大于一切样式
>
 **权重计算规则****:**
>
> 内联样式:style=””-----权值1000
>
> ID选择器:  #ID   -----权值100
>
> 类/伪类/属性选择器 -----权值10
>
> 类型选择器和伪元素 :div/p------权值1
>
> 继承的样式没有权值
>
**☆CSS3新特性和伪类有哪些?** 
> 
> border-radius(圆角)
>
> box-shadow(阴影)
> 
> text-shadow(文字阴影)
> 
> 线性渐变(line-gradient)
> 
> transform各种样式(旋转/缩放/定位[xyz]/倾斜)
> 
> 增加了更多的CSS旋转武器,背景颜色加入了rgba
>   
> Border-images/媒体查询/多栏布局
>
**☆CSS3新特性和伪类有哪些?** 
>
> P: first-of-type 选择属于其父元素中的同类型的第一个P元素
>
> P:last-of-type 选择其父元素中的同类型的最后一个P元素
>
> ::after/::before在元素之前或之后添加内容
>
> ::disabled   控制表单控件的禁用状态
>
> ::checked   单选框或复选框被选中  
>
 **less的一些优势。**
>
> \1. 结构清晰，便于扩展
>
> \2. 可以方便的屏蔽浏览器私有语法差异
>
> \3. 可以轻松实现多重继承
>
> \4. 完全兼容CSS代码，可以方便的应用到老项目中。Less知识在CSS语法上做了扩展，所以老的CSS代码也可以与Less代码一同编译
> 缺点：必须要编译，无论在客户端还是服务器端，都是一种额外的花销
>
>

> 
**水平居中**
> text-align:center;
> 
> margin: 0 auto;
>
**垂直居中**
> 
> 文本垂直：height和line-height一样
> 
>display:flex,align-item:center
>
**水平垂直居中**
```
固定宽高的
1.margin根据已知的宽高写死
2.父级relative定位+子级absolute定位+margin-top(负的高度一半)
+margin-left(负的宽度的一半)+left:50%;top:50%
        .box-container{
        position: relative;
            width: 300px;
        height: 300px;
    }
    .box-container .box {
        width: 200px; 
        height: 100px;
        position: absolute; 
        left: 50%; 
        top: 50%;
        margin-top: -50px;    /* 高度的一半 /
        margin-left: -100px;    / 宽度的一半 */
    }
设置父元素的position为相对定位，子元素绝对定位，并在 top 和 left 方向上移动父元素50%的距离。
但这个时候，是子元素的上边框和左边框距离父元素150px，整体向右下角偏了一些，所以还需要再用 margin 调整至中心位置，数值分别是高度和宽度的一半。

二、未知宽高
1、transform 方案: 存在兼容问题：
    .box {
        position: relative; 
        left: 50%; 
        top: 50%;
        transform: translate(-50%, -50%);    
    }
2、flexbox 方案: 
    .box-container {
        display: flex;
        justify-content: center;
        align-items: center;
    }
设置父元素为 flex 弹性盒模型，
并在主轴和副轴上设置居中
3、display: table-cell 无兼容性问题
    .box {
        position: relative;
        width: 300px;
        height: 300px;
        border: 1px solid red;
        display: table-cell;    
        text-align: center;    
        vertical-align: middle;
    }
只需要设置父元素即可，
text-align: center; 
并在竖直方向上令内容居中（middle），
早期属性，不存在兼容问题。
3、定位 + margin   
 .box-container{       
 position: relative;   
 }    
.box {        
width: 100px;       
 height: 100px;      
  position: absolute;        
 left: 0;         
top: 0;        
 right: 0;        
 bottom: 0;        
margin: auto;    }
未知高度：同样是使用绝对定位，但四个方向的偏移量全都为0，之后设置 margin:auto 分配剩余空间，令元素的均匀拖拽至父元素的中心位置。
```
**Display有哪些哪些值?说明他们的作用**
>
> block   元素转化为块级元素
>
> inline    元素转化为行内元素
>
> inline_block  元素转化问行内块元素
>
> None     次元素不会显示,脱离文档流
>
> List-item  元素转化为行内样式,并添加列表样式(如UL下的li)
>
> Table   元素会以块级表格来显示
>
> Inherit   继承父元素display属性
>
**Position的值?**
>
> Relative  相对定位(相对于原来位置定位,不脱离文档流)
>
> Absolute  绝对定位(相对于他最近的定位父元素定位,脱离文档流)
>
> Fixed   窗口定位(相对于浏览器窗口进行定位,脱离文档流)
>
> Static ['stætɪk]  默认值,不定位
>
> Inherit    继承父元素的position属性
>
 **flex布局以及常用属性**
>
> flex布局可以完美实现响应式布局
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/DEA78D57A0BC4DDD9588888A912E6E6C/4563](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/DEA78D57A0BC4DDD9588888A912E6E6C/4563)
>
> 
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/09F28B82E7104B3EA27B95A83277DF0C/4562](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/09F28B82E7104B3EA27B95A83277DF0C/4562)
>
> 
>
 **请解释一下****CSS3的flexbox(弹性盒布局模型),以及适用场景?**
>
> 是一个用于页面布局的新CSS功能 ,规定框内的子元素是否可以伸缩器尺寸
>
**CSS打造三角形?**
>
> 宽度0,高度0,边框加宽,给一边加颜色,其余三边使用transparent
>
**满屏品字布局****?**
>
> 上面div宽度100%;
>
> 下面两个宽度width50%+float/display:inline/inlin-block;
>
**li与li之间有看不见的空白间隙是什么原因引起来的?**
>
> 行内块排列会受到(空格/回车)等的影响,因为空格也属于字符,把字符大小 设置为0就ok了
>
**为什么要初始化****css样式?**
>
> 浏览器的兼容性问题,有些浏览器对标签的默认值是不一样的,如果没有 设置CSS初始化,浏览器之间的页面会有差异,最简单的方式:
>
> *{ padding ; 0 ;   margin : 0 ; }
>
 **CSS中的visibility属性的collapse[kə'læps]属性是干嘛的?**
>
> 1、一般情况和visibility：hidden一样，不脱离文档流
>
> 2、在table的tr元素，脱离文档流
>
> 3、在table的td元素中，不脱离文档流
>
**外边距合并是指的什么意思****?**
>
> 是指两个垂直的margin相遇,会合并在一起,margin高度是以最大的margin值为准;
>
**移动端的布局用过媒体查询吗****?**
>
> 媒体查询主要用于响应式页面,媒体查询通过页面浏览设备的窗口宽度,完成相应的样式
>
> <style>@media(min-width)and(max-width){样式}</style>
>
> 拓展问题:
>
 **响应式页面****?**
>
> 响应式页面主要为了配合各种用户设备的窗口宽度,主要用得到的一个是媒体查询,一个是bootstrap,一个是rem单位,rem根据页面字体大小等比缩放,可以用vw/vh+rem,vw/vh是将窗口大小平分为100份;
>
> ﻿[**CSS媒体查询的原理是什么？**](https://segmentfault.com/q/1010000011514232)﻿
>
> 窗口的onresize事件，得到窗口大小匹配对应的样式修改
>
**CSS预处理器(sass和less)用过吗?**
>
> 个人比较喜欢less,结构清晰,可以与html结构保持一致,省去了css多层选择器的用法
>
**使用****CSS预处理的优缺点分别是什么？**
>
> 优点：
>
> 提高CSS可维护性
>
> 易于编写嵌套选择器
>
> 引入变量，增添主题功能。可以在不同的项目中共享主题文件。
>
> 缺点：
>
> 需要预处理工具
>
> 重新编译的时间可能会很慢
>
**CSS优化/提高性能的方法有哪些?**
>
> 使用css预处理器(less/sass),增加代码可复用性,方便项目的协作开发,可维护性.
>
**Margin与padding的区别?**
>
> Margin是控制元素与元素之间的距离,padding是分元素与内容之间的距离
>
**Css如何实现横向滚动与竖向滚动?**
>
> 横向滚动:父元素:overflow-x:auto; overflow-y:hidden;
>
> 竖向滚动:父元素 overflow-x:hidden;overflow-x:auto;
>
**如何设置滚动条样式****?**
>
> Scrollbar样式属性,有很多种,很少用,单词没怎么记住;
>
**视觉差效果是如何实现的****?**
>
> 给背景图片添加background-attachment:fixed属性,将背景固定在窗口,在使用background-position:top center或0% 0%;后续可以通过js修改background-position的top值,实现背景图片跟随页面上下移动的效果
>
**你对****line-height如何理解?**
>
> line-height是设置杭行高的style样式,可以增加设置文本行与行之间的上下间距,也可以实现文本在div中的垂直居中
>
**设置元素浮动后****,元素的display值是什么吗?**
>
> 浮动后,元素的display值自动变为display:block;
>
**怎么让****chrome支持小于12px的文字?**
>
> 一个是使用图片,不知道的话,就说12号字体基本就已经是浏览器的自小号字体,如果字太小,用户阅读内容会很容易产生视觉疲劳感,所以页面中通常是使用12px或者大于12px的字体,比如:16/18/24/32号字体,是比较常用的字体大小
>
**如何设置字体斜体****?**
>
> i标签/em标签/font-style: oblique[ə'blik]
>
**如果需要手写动画****,最小时间间隔是多少?**
>
> 显示器默认60Hz,一秒刷新60次,1000/60,约为16.7ms
>
**有一个高度自适应的****div,里面有两个div,一个高度100px,一个如何自适应高度?**
>
> 1/父元素box-sizing:border-box;padding-top:100px;position:relative;
>
> 第一个div   position:absolut;
>
> 第二个div  height:100%;
>
 **Png/jpg/gif这些图片格式解释一下?**
>
> jpg是正常的图片格式/png主要设置无背景图片/gif是动态图片
>
 **Style标签写在body前还是body后?** 
>
> 正常是写在body前的,而且style也可以body中,但是这回导致CSS重新渲染一次页面,占用一定的时间
>
**有什么不同的方式可以隐藏内容****?**
>
> visibilty：hidden：元素任然在文档流中，并占用空间；
>
> display：none：元素脱离文档流，不占用空间；
>
> position：left：-999999px：将内容至于屏幕之外
>
> text-index：-9999：只适用于block元素中的文本
>
**消除****transition闪屏**
>
> .css {
>
> ​    -webkit-transform-style: preserve-3d;
>
> ​    -webkit-backface-visibility: hidden;
>
> ​    -webkit-perspective: 1000;
>
> }
>
> 过渡动画（在没有启动硬件加速的情况下）会出现抖动的现象，以上的解决方案只是改变视角来启动硬件加速的一种方式；
>
> 启动硬件加速的另外一种方式：
>
> .css {
>
> ​      -webkit-transform: translate3d(0,0,0);
>
> ​      -moz-transform: translate3d(0,0,0);
>
> ​      -ms-transform: translate3d(0,0,0);
>
> ​      transform: translate3d(0,0,0);
>
> ​    }
>
> 启动硬件加速最常用的方式：translate3D，translateZ，transform
>
> opacity属性/过渡动画(需要动画执行的过程中才会创建合成层，动画没有开始或结束后元素还会回到之前的状态)
>
> will-chang属性（这个比较偏僻），一般配合opacity使用（而且经测试，除了上述可以引发硬件加速的属性外，其它属性并不会变成复合层）
>
> 弊端：硬件加速会导致CPU性能占用量过大，电池电量消耗加大；因此，尽量避免泛滥使用硬件加速。
>
**CSS实现单行文本移除显示...**
>
> overflow : hidden ;
>
> text-overflow : ellipsis ;
>
> white-space : nowrap ;
>
> 还需要加宽度width属性来兼容部分浏览器
>
**实现多行文本溢出显示****...**
>
> display : -wedkit-box ;
>
> -webkit-box-orient : vertical ;
>
> -webkit-line-clamp : 3 ;
>
> overflow : hidden ;
>
> 适用范围 : 因使用了Webkit的CSS扩展属性,该方法适用于Webkit浏览器以及移动端
>
> 注:
>
> -webkit-line-clamp用来限制在一个块元素显示的文本的行数,为了实现该效果,它需要组合其它的webkit属性。
>
> 常见结合属性：
>
> display：-webkit-box； 必须结合的属性，将对象作为弹性伸缩盒子模式显示。
>
> -webkit-box-orient  必须结合的属性，设置或减缩伸缩盒对象的子元素排列方式。
>
> **溢出显示。。。的另外一种显示方式**
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/25B852C2F08F42B9BDDCAE6A335ADC38/4571](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/25B852C2F08F42B9BDDCAE6A335ADC38/4571)
>
> 
>
> 实现方式：
>
> div{
>
> position：relative；
>
> line-height：20px；
>
> max-height：40px；
>
> overflow：hidden；
>
> }
>
> div：after{
>
> content : “...”;
>
> position : absolute ;
>
> bottom : 0 ;
>
> right : 0 ;
>
> padding-left : 40px ;
>
> background : -webkit-linear-gradient(left , transparent , #fff  55%);
>
> background : -o-linear-gradient(left , transparent , #fff  55%);
>
> background : -moz-linear-gradient(left , transparent , #fff  55%);
>
> background : linear-gradient(left , transparent , #fff  55%);
>
> }
>
> 此方法也有弊端：就是未超出行的情况下也会出现省略号
>
> 注:
>
> \1. 将height设置为line-height的整数倍,防止超出的文字露出。
>
> \2. 给p::after添加渐变背景可避免文字只显示一半。
>
> \3. 由于ie6-7不显示content内容，所以要添加标签兼容ie6-7，兼容ie8需要将 ：：after替换成 ：after
>
**让图文不可复制** TODO
>
> -webkit-user-select：none；
>
> -ms-user-select：none；
>
> -moz-user-select：none；
>
> -khtml-user-select：none；
>
> user-select：none；
>
> 这些网页为了尊重原创，复制的文本都会被加上一段来源说明，这个是如何做到的呢？拓展：
>
> 大致思路：
>
> \1. 答案区域监听copy事件，并阻止这个事件的默认行为。
>
> \2. 获取选中内容（window.getSelection( )）加上版权信息，然后设置到剪切板（clipboardata.setData( )）
>
 **visibility：hidden与display：none的区别？**
>
> 两个css样式都有隐藏元素的效果，但是它们的区别在于：display：none隐藏元素，可以脱离文档流，而visibility隐藏的元素不会脱离文档流，会占有原来的位置。
>
**em，rem，px的区别？**
>
> **px像素单位**-----相对长度单位，相对于显示屏分辨率。
>
> **特点：**IE无法调整那些使用px作为单位的字体大小
>
> 国外的大部分网站能够调整的原因在于其使用了em或rem作为字体单位
>
> Firefox能够调整px和em、rem，但是96%以上的中国网民使用IE浏览器或（内核）
>
>**em**-------相对长度单位，相对于当前对象内文本的字体尺寸。如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸（浏览器的默认字体大小是16px。未经调整的浏览器都符合1em = 16px）
>
> **特点：**em的值不是固定的
>
> em会继承父级元素的字体大小
>
> **rem**-----rem是CSS3新增的一个相对访问（root em，根em），这个单位引起了广泛关注。rem与em的区别在于使用rem为元素设定字体大小时，仍然是相对大小，但相对的是HTML根元素。这个单位可以根据修改根元素就成比例的调整字体大小。可避免字体大小逐层复合的连锁反应。注意：根节点的字体大小需要动态设置，一般是屏幕的宽度/经验值（你自己定义）
>
**css动画与js动画的差异**
>
> \1. js动画代码相对复杂一些
>
> \2. 动画运行时，对动画的控制程度上，js能够让动画暂停、取消、终止，css动画不能添加事件
>
> \3. 动画性能看，js动画多了一个js解析的过程，性能不如css动画好
>
**何让一个元素垂直****/水平（垂直水平）都居中，请列出你能想到的几种方式？**
>
 · 水平垂直居中 —— **方式一**
>
> <div class="div-demo"></div>
>
 ```
 .div-demo{

 ​    width:100px;

 ​    height:100px;

 ​    background-color:#06c;

 ​    margin: auto;

 ​    position:absolute;

 ​    top: 0;

 ​    left: 0;

 ​    bottom: 0;

 ​    right: 0;

 }
 ```
>
> · 水平垂直居中 —— **方式二**
```
.div-demo{
 ​    width:100px;

 ​    height:100px;

 ​    background-color:#06c;

 ​    margin: auto;

 ​    position:absolute;

 ​    top: 50%;

 ​    left: 50%;

 ​    transform: translate(-50%,-50%);

 ​    -webkit-transform: translate(-50%,-50%);

 }
>
```
> 
> · 水平垂直居中 —— **方式三**，（新旧伸缩盒兼容）
>
> <body class="container">
>
>   <div class="div-demo"></div>
>
> <style>
> 
>
>
> ​    **html**,**body**{
>
> ​      height:100%;
>
> ​    }
>
> ​    .container{
>
> ​      display: box;
>
> ​      display: -webkit-box;
>
> ​      display: flex;
>
> ​      display: -webkit-flex;
>
> ​      -webkit-box-pack: center;
>
> ​      -webkit-justify-content: center;
>
> ​      justify-content: center;
>
> ​      -webkit-box-align: center;
>
> ​      -webkit-align-items: center;
>
> ​      align-items: center;
>
> ​    }
>
> ​    .div-demo{
>
> ​      width:100px;
>
> ​      height:100px;
>
> ​      background-color:#06c;
>
> ​    }
>
> </style>
>
> </body>
>
**Chrome、Safari等浏览器，当表单提交用户选择记住密码后，下次自动填充表单的背景变成黄色，影响了视觉体验是否可以修改**
>
**input**:-webkit-autofill, **textarea**:-webkit-autofill, **select**:-webkit-autofill {
>
> background-color: #fff;//设置成元素原本的颜色
>
> background-image: none;
>
> color: rgb(0, 0, 0);
>
> }
>
> //方法2：由(**licongwen** )补充**input**:-webkit-autofill {
>
> -webkit-box-shadow: 0px 0 3px 100px #ccc inset; //背景色
>
> }
>
**浏览器的最小字体为****12px，如果还想再小，该怎么做？**
>
> · 用图片：如果是展示的内容基本是固定不变的话，可以直接切图兼容性也完美(不到万不得已，不建议);
>
> · 找UI设计师沟通：为了兼容各大主流浏览器，避免后期设计师来找你撕逼，主动找TA沟通，讲明原因 ————注意语气，好好说话不要激动，更不能携刀相逼;
>
> · CSS3：css3的样式transform: scale(0.7)，scale有缩放功能;
>
> · 又去找[chrome](https://www.toutiao.com/i6606779850801807885/)复习了一下，说是 “display:table;display: table-cell;” 可以做到，没用过。
>
**给一个****div设置它的宽度为100px，然后再设置它的padding-top为20%。问：现在这个div有多高？**
>
> 这题主要考察了对w3c标准的了解。如果你亲自去浏览器去试的话会发现这个div的高为：316.8(注意：不同分辨率的电脑测试会有不同的效果，这里以我的电脑1600x900为参考)，其实到这里这题已经是解开了，但是可能还有些同学没明白这个316.8是如何计算得来的。别急，请听我细细道来。
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/0712D0F796C647C78667F53EC2E8D361/4579](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/0712D0F796C647C78667F53EC2E8D361/4579)
>
> 
>
> 如果你搞不懂结果为何是这个的话可能会去查[w3school](http://link.zhihu.com/?target=http://www.w3school.com.cn/cssref/pr_padding.asp)，你可能会看到：
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/EA07A04354584C6F84130C1F12A30B2C/4570](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/EA07A04354584C6F84130C1F12A30B2C/4570)
>
> 
>
> 但是可以这么说上面的所说的是错的，或者说，表述不准确。
>
> 例如一下情况：
>
> //css
>
> .inner{
>
> ​    position: absolute;
>
> ​    width: 100px;
>
> ​    padding-top: 20%;
>
> }
>
> .mid{
>
> width: 200px;
>
> }
>
> .wrap{
>
> position: relative;
>
> width: 300px;
>
> }
>
> //html
>
> <div class="wrap">
>
>     <div class="mid">
>
>         <div class="inner"></div>
>
> </div>
>
> </div>
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/8C15F417E1064F84B983F4B1B7CF57B0/4580](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/8C15F417E1064F84B983F4B1B7CF57B0/4580)
>
> 
>
> 如果按照[w3school](http://link.zhihu.com/?target=http://www.w3school.com.cn/cssref/pr_padding.asp)说的，这个inner的高应该是40px，但是实际不是，而是60px，是以wrap的宽度计算的，由此可见，w3school的说法不成立。
>
> 那么，当padding设置为%时到底以谁为参考呢？
>
> 事到如今我也不给大家卖关子了，其实是以[包含块](http://link.zhihu.com/?target=http://www.ayqy.net/doc/css2-1/visudet.html%23containing-block-details)为参考的。通俗点来说就是谁包含它，它就以谁为参考，在这里inner设置了position:absolute脱离了原来的文档流，就会去寻找它的祖先元素设置了position:relative的元素作为它的包含块。如果还不懂包含块是啥的同学建议仔细阅读我刚刚给的链接，同时还可以参考我在[segmentfault](http://link.zhihu.com/?target=https://segmentfault.com/q/1010000008362925)上的这个问题。
>
**写一个左中右布局，占满全屏，其中左右两块的固定宽度是****200，中间自适应宽度，请写出结构及样式：**
>
> <style>
> 方法一：
>
> html,body{ margin:0;width:100**%**; }
>
> h3{ height: 100**px**; margin: 20**px** 0 0; }
>
> *#left*,*#right*{ width:200**px**;height: 200**px**;background: **#****000**; position: absolute;top: 120**px**;}
>
> *#left*{left:0**px**;}
>
> *#right*{right: 0**px**;}
>
> *#center*{margin:2**px** 210**px** ;background-color: **#****eee**;height: 200**px**; }
>
> </style>
>
> <style>
>
> 方法二：
>
> div{
>
> height: 300**px**;
>
> }
>
> *#left*,*#right*{
>
> width: 200**px**;
>
> background: **#****000**;
>
> }
>
> *#left*{
>
> float:left;
>
> }
>
> *#right*{
>
> float:right;
>
> }
>
> *#center*{
>
> margin-left:200**px**;
>
> margin-right:200**px**;
>
> }
>
> 
>
> </style>
>
> 
>
> 
>
> <h3>实现三列宽度自适应布局</h3>
>
> <div id="left">左边</div>
>
> <div id="right">右边</div>
>
> <div id="center">中间</div>
>
> 使用左右浮动的方式相对于绝对定位的方法会有一点差异性，并且会有一点小bug，当中间部分小于内容的情况下，会将右侧的内容挤至下方，可自己试试对比。
>
> **CSS sprite是什么？有什么优缺点？**
>
> 精灵图，将多个小图片拼接到一个图片中。通过background-position和元素尺寸调节需要显示的背景图案
>
> 优点：
>
> 减少http请求数，极大的提高页面加载速度
>
> 增加图片信息重复度，提高压缩比，减少图片大小
>
> 更换风格方便，只需在一张或几张图片上修改颜色或样式即可实现
>
> 缺点：
>
> 图片合并麻烦
>
> 不方便维护
>
> **什么是****FOUC？如何避免**
>
> flash of Unstyle Content：用户定义样式表加载之前浏览器使用默认样式显示文档，用户样式加载渲染之后再从新显示文档，造成页面闪烁
>
> **解决方法：**把样式表放到文档的head中
>
> **为什么要初始化****CSS样式？**
>
> 因为浏览器的兼容性问题，不同浏览器对有些标签的默认值是不同的，如果没有css初始化往往会出现浏览器之间的页面显示差异
>
> 初始化样式会对SEO有一定的影响，但鱼和熊掌不可兼得，但力求影响最小的情况下初始化
>
> **在网页中的字体大小应该使用偶数还是奇数？为什么呢？**
>
> 偶数字号相对更容易和web设计的其他部分构成比例关系
>
> **如果需要手动写动画，你认为最小时间间隔是多久？为什么？（阿里）**
>
> 多数显示器默认频率是60Hz，即1秒刷新60次，所以理论上最小间隔1/60*1000ms = 16.7ms
>
> **CSS在性能优化方面的方法？**
>
> css压缩与合并、Gzip压缩
>
> css文件放在head中，不要使用@import
>
> 尽量用缩写、避免用滤镜、合理使用选择器
>
> **base64的原理及缺点**
>
> 优点：可以加密，减少了http请求
>
> 缺点：需要消耗CPU进行编解码
>
> **stylus、sass、less区别**
>
> 均具有变量、混合、嵌套、继承、颜色混合五大基本特性
>
> Sass和Less语法较为严谨，Less要求一定要使用大括号{ }，Sass和Stylus可以通过缩进表示层次与嵌套关系
>
> Sass无全局变量的概念，Less和Stylus有类似于其他语言的作用于概念
>
> Sass是基于Ruby语言的，而Less和Stylus可以基于NodeJS NPM下载相应库就进行编译
>
重绘回流
