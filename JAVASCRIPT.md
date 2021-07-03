**前端开打掌握的知识内容概要**

**HTML/CSS:** 

对web标准的理解(结构/表现/行为)、浏览器内核、渲染原理、依赖管理、兼容性、CSS语法、层次关系、常用属性、布局、 选择器、权重、盒模型、Hack、CSS预处理器、Flexbox、CSS Modules、Document flow、BFC、HTML5（离线&储存&history、多媒体、webGL、SVG、Cavas）

**Javascript：**

数据类型、运算、对象、function、继承、闭包、  作用域、原型链、事件、prototype、RegExp、JSON、Ajax、DOM、BOM、内存泄漏、跨域、异步请求、模板引擎、模块化、Flux、同构、算法、ECMAScript6、Nodejs、HTTP、前端MVC、MVVM、路由、模块华、Canvas、ECMAScript

**其他：**

主流MVVM框架(React\Vue\Angular)、Hybrid App\React Native\Weex、TypeScript、RESTFul、WEB安全、前端工程化、依赖管理、性能优化、重构、团队协作、可维护、易用性、SEO、UED、前端技术选型、快速学习能力等；

 
**JS:**

 **JS数据类型有哪些?**

 栈: (原始数据) string/number/boolean/null/undefined/symbol
 堆: (引用数据类型)object(function,Date,Array,正则对象)

 数据类型一共7（6种基本类型+1种引用类型）种

**介绍****JS有哪些内置对象？**

 object是Javascript中所有对象的父对象
 数据封装类对象：Object、Array、Boolean、Number和String
 其他对象：Function、Arguments、Math、Date、RegExp、Error

**JS几种常见内置对象和方法**
```
Array对象中常用方法： 
concat（）　　　　 表示把几个数组合并成一个数组
join（）　　　　　  设置分隔符连接数组元素为一个字符串
pop（）　　　　　  移除数组最后一个元素
shift（）　　　　　 移除数组中第一个元素 
unshift()          往数组里面加元素
push（）　　　　    往数组中新添加一个元素，返回最新长度
slice（start，end）  返回数组中的一段
splice（）　　　　  可以用来删除，可以用来插入，也可以用来替换 
sort（）　　　　　  对数组进行排序
reverse（）　　　　反转数组的顺序 
toLocaleString()　　 把数组转换为本地字符串
array对象属性： 
length　　　　　　  表示取得当前数组长度 （常用）
constructor　　　　 引用数组对象的构造函数
prototype　　　　　通过增加属性和方法扩展数组定义

Object对象常用方法
静态方法
Object.assign() 
Object.create() 创建对象并且将该对象的原型指向传入的参数
Object.defineProperty()   给对象添加一个属性并指定他的配置
Object.defineProperties() 给对象添加多个属性并指定她们的配置
Object.entries()   返回给定对象自身可枚举属性的 [key, value] 数组
Object.values()    返回给定对象自身可枚举值的数组
Object.is()     判断两个值是否相等
Object.freeze()  冻结对象：其他代码不可以删除或者更改对象
Object.seal()  封闭对象：其他代码不可以删除增加属性，但是对原有属性是可以更改的。
Object.isSeal() 判断对象是否已经封闭
Object.isFreeze() 判断对象是否已经冻结
Object.getPrototypeOf()  返回指定对象的原型对象
Object.setPrototypeOF()  设置对象的原型
Object.getOwnPropertyNames() 返回数组，包含指定对象的所有可枚举和不可枚举的属性名
Object.getOwnPropertySymbols() 返回一个数组，它包含了指定对象自身所有的符号属性
Object.getOwnPropertyDescriptor() 返回对象指定的属性配置
Object.isExtensible() 判断对象是否可扩展。
Object.preventExtensions() 防止对象的任何扩展。方法让一个对象变的不可扩展，也就是永远不能再添加新的属性。

String对象 
charAt()　　　　　 　　　　返回指定索引的位置的字符 
indexOf() 　　　　  　　　　从前向后检索字符串，看是否含有指定字符串 Boolean
lastIndexOf()　　　 　　　　从后向前检索字符串，看是否含有指定字符串 Boolean
concat()　　 　　　　　　　连接两个或多个字符串
match()　　     　　　　　　使用正则表达式模式对字符串执行查找，并将包含查找结果最为结果返回
replace()　　　　　　　　　替换一个与正则表达式匹配的子串
search()　　　　　　　　　 检索字符串中与正则表达式匹配的子串。如果没有找到匹配，则返回 -1。 
slice（start，end） 　　　　根据下表截取子串 
substring（start，end）　　 根据下表截取子串 
splite()　　　　　　　　　　  根据指定分隔符将字符串分割成多个子串，并返回数组
substr(start，length)　　　　根据长度截取字符串 
toUpperCase()　　　　　　 返回一个字符串，该字符串中的所有字母都被转化为大写字母。 
toLowerCase()　　　　　　 返回一个字符串，该字符串中的所有字母都被转化为小写字母。
trim（）：                移除字符串两边的空格


Math对象
ceil()向上取整。
floor()向下取整。
round()四舍五入。
random()取随机数


Date对象
getDate函数：返回天，值为1～31。
getDay函数：返回星期，值为0～6，0表示星期日。
getHours函数： 返回小时，值为0～23。
getMinutes函数：返回分钟，值为0～59。
getMonth函数： 返回月，值为0～11。
getSeconds函数：返回秒，值为0～59。
getTime函数：返回系统时间。
getTimezoneOffset函数：　返回此地区的时差(当地时间与GMT格林威治标准时间的地区时差)，单位为分钟。
getYear函数：返回日期的“年”部分。返回值以1900年为基数，如1999年为99。
parse函数：返回从1970年1月1日零时整算起的毫秒数(当地时间)。
setDate函数：设定天，值为0～31。setHours函数：设定小时，值为0～23。setMinutes函数： 设定分钟，值为0～59。
setMonth函数：设定月，值为0～11。其中0表示1月，...，11表示12月。
setSeconds函数： 设定秒，值为0～59。
setTime函数：设定时间。时间数值为1970年1月1日零时整算起的毫秒数。 
setYear函数：设定年。
toGMTString函数：转换日期成为字符串，为GMT格林威治标准时间。
setLocaleString函数：转换日期成为字符串，为当地时间。 
UTC函数： 返回从1970年1月1日零时整算起的毫秒数(GMT)。
```

**如何转化类型****?**

 转浮点数parseFloat();
 转字符串toString()/string()
 数组转字符串 join();
 字符串转数组: split();
 总结：join和split是逆运算的感觉
```
join();
const elements = ['Fire', 'Air', 'Water'];
console.log(elements.join());
// expected output: "Fire,Air,Water"
console.log(elements.join(''));
// expected output: "FireAirWater"
console.log(elements.join('-'));
// expected output: "Fire-Air-Water"

split()
const str = 'The quick brown fox jumps over the lazy dog.';
const words = str.split(' ');
console.log(words[3]);
// expected output: "fox"

const chars = str.split('');
console.log(chars[8]);
// expected output: "k"

const strCopy = str.split();
console.log(strCopy);
// expected output: Array ["The quick brown fox jumps over the lazy dog."]

```
**栈与堆的区别**
 栈与堆的储存位置不同;
 原始数据是储存在栈中简单数据段,体积小,大小固定,属于频繁使用的数据.
 引用数据类型是储存在堆中的对象,占据的空间大,如果储存在栈中会影响运行性能,引用数据类型在栈中指明了自己的所在地.当代码解析时,会先从栈中获取地址,然后再从堆中获取实体;
**作用域：**
每一个变量、函数都有其作用的范围，超出范围不得使用，这个叫做作用域

**作用域链：**
 查找变量的过程。先找自己局部环境内部有没有声明或者是函数，如果有，则查看声明有无赋值或者是函数的内容，如果没有，则向上一级查找。
**什么是面向对象编程及面向过程编程，他们的异同和优缺点**

 面向过程就是分析出解决问题所需要的步骤，然后用函数吧这些步骤一步一步实现，使用的时候一个一个一次调用就可以了

 面向对象是把构成问题事务分解成各个对象，建立对象的目的不是为了完成一个步骤，而是为了描述某个事物在整个解决问题的步骤中的行为

 面向对象是以功能来划分问题，而不是步骤

**面向对象编程思想**

 基本思想是使用对象、类、继承、封装等基本概念来进行程序设计

 优点：易维护

 \- 采用面向对象思想设计的结构，可读性高，由于继承的存在，即使改变需求，那么维护起来是非常方便你和较低成本的

 易扩展

 开发工作的重用性、继承性高、降低重复工作量

 缩短了开发周期

**如何解释****this在js中起的作用?**

 Js中的this,一般取决于调用这个函数的方法

 1/如果函数被实例化(new 构造函数名())的情况下,this指向全新的对象

 2/如果是某标签触发什么事件,调用了这个函数,this指向标签(整个DOM节点,包含它的子元素);TODO

 3/如果函数使用了call/apply,this是作为参数传入对象

 4/有时候this指向不明确的话,this会指向window,
 
 5/ES6中的箭头函数修改了this指向,永远指向作用域
**js中this的用法（经典）：**TODO
this指向被函数调用的那个对象
 
☆**说说****JS原型和原型链**

**原型**：
函数都有prototype(显示原型)属性，而prototype会自动初始化一个空对象，这个对象就是原型对象

 原型对象中会有一个constructor属性,这个属性将指向了函数本身

 实例化对象都有一个_proto_(隐式原型)属性，_proto_属性指向原型对象

**原型链：**从实例对象往上找构造这个实例的相关对象，然后这个关联的对象再往上找，找到创造它的上一级的原型对象，以此类推，一直到object.prototype原型对象终止,原型链结束.

**构造函数**
专门用来生成
​实例对象的函数，既对象的模板：类
JavaScript 语言的对象体系，不是基于“类”的，而是基于构造函数（constructor）和原型（prototype）

**原型链中的原型对象中的内容****,是会被不同的实例,所共有的**

 |      |                                                              |
 | ---- | ------------------------------------------------------------ |
 |      | ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/F684CF201B0846D4A35D835BB9DDA279/4567](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/F684CF201B0846D4A35D835BB9DDA279/4567) |

 

**如何准确判断一个变量是引用类型****?**

 1.instanceof用于判断引用类型属于哪个构造函数的方法

 var arr = [];

 arr  instanceof  Array;  //true


 **原理****:**

 ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/4EE1CD020C6949B38C29316A30226C4B/4576](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/4EE1CD020C6949B38C29316A30226C4B/4576)

 

 instanceof是用来判断实例的_proto_和构造函数的prototype是否指向一个原型对象，

 但是有一个弊端，只要出现在一条原型链上的，都会返回true（每个函数都有prototype，每个对象都有一个内部属性__proto__，其指向它的原型对象。原型对象也是一个对象，所以也有__proto__）

2.constructor

 这个时候要用实例__proto__.constructor更加严谨
会有问题，因为实例是通过__proto__指向构造函数的原型对象来找到constructor。如果改写了构造函数的原型，或者改写了构造函数的constructor。都会让这种方法出错。
 var arr = [ ];

 console.log(arr instanseof Array);  //true

 console.log(arr.__proto__.constructor === Array)  //true

**如何判断数组类型**

Array.isArray()

Object.prototype.toString.call(text) === '[object Array]'

**☆call和apply以及bind的区别和作用?**

 apply和call都是调用一个对象的一个方法，用另一个对象替换当前对象。

 相同点：方法的含义是一样的，即方法功能是一样的。并且第一个参数的作用是一样的

 不同点：call可以传入多个参数、apply只能传入两个参数，所以其第二个参数往往是作为数组形式传入

 存在意义：实现（多重）继承
 bing是返回一个新的函数，不会改变原始函数的this指向


**继承的方法有哪些？能具体说说嘛**TODO

 原型链继承、构造继承、实例继承、拷贝继承、组合继承、寄生组合继承

**继承详情解释：**

 既然要实现继承，那么我们首先要有一个父类，代码如下:

 //先定义一个父类

 function Animal(name){

 //属性

 this.name = name || 'Animal';

 //实例方法

 this.sleep = function(){

 console.log(this.name + "正在睡觉!")

 }

 }

 //原型方法

 Animal.prototype.eat = function(food){

 console.log(this.name + "正在吃" + food);

 }


**☆什么是闭包？闭包有什么作用？**

 由于在js中，变量到的作用域属于函数作用域，在函数执行后作用域会被清除、内存也会随之被回收，但是由于闭包是建立在一个函数内部的子函数，由于其可访问上级作用域的原因，即使上级函数执行完，作用域也不会随之销毁，这时的子函数---也就是闭包，便拥有了访问上级作用域中的变量权限，即使上级函数执行完后，作用域内的值也不会被销毁。

 闭包解决了什么：在本质上，闭包就是将函数内部和函数外部连接起来的一座桥梁。

 由于闭包可以缓存上级作用域，那么就使得函数外部打破了“函数作用域”的束缚，可以访问函数内部的变量。以平时使用的Ajax成功回调为例，这里其实就是个闭包，由于上述的特性，回调就拥有了整个上级作用域的访问和操作能力，提高了几大的便利。开发者不用去写钩子函数来操作审计函数作用域内部的变量了。

 闭包有哪些应用场景：

 闭包随处可见，一个Ajax请求的成功回调，一个事件绑定的回调函数，一个setTimeout的延时回调，或者一个函数内部返回另一个匿名函数，这些都是闭包。简而言之，无论使用何种方式对函数类型的值进行传递，当函数在别处被调用时都有闭包的身影

 闭包的缺陷：由于闭包打破了函数作用域的束缚，导致里面的数据无法清除销毁，当数据过大时会导致数据溢出

当函数可以记住并访问所在的词法作用域时，就产生了闭包，即使函数是在当前词法作用域之外执行。
在定时器、事件监听器、ajax请求，跨窗口通信、web Workers或者任何其他的异步（或者同步）任务中，只要使用了回调函数，实际就是在使用闭包

**事件代理（事件委托）****:**TODO

 事件代理是将子元素的事件写一个父元素,让父元素代替处理,内部使用e.target,e.target就是触发这个事件的子元素

**事件的各个阶段**

 捕获阶段  ---  目标阶段  ---  冒泡阶段

 document  ---  target目标  ---  document

 由此addEventListener的第三个参数设置为true和false的区别已经非常清晰了

 true---代表该元素在事件的”捕获阶段”(由外向内传递)响应事件

 false ---表示该元素在事件的”冒泡阶段”(由内向外传递)响应事件

**☆new操作符在创建实例的时候经历了哪几个阶段**TODO


```
<!-- 
1.创建一个新对象
2.将构造函数的作用域赋给新对象(因此this就指向了这个新对象)
3.执行构造函数的代码。(为这个新对象添加属性)
4.返回新对象
 --


function newOperation(constructFunc) { 
    const newObj = Object.create(constructFunc.prototype); 
    constructFunc.call(newObj); 
    return newObj; 
}
```

**异步编程的实现方式**

```
-1.回调函数
 优点：简单、容易理解
 缺点：不利于维护，代码耦合高
-2.事件监听（采用时间驱动模式，取决于某个事件是否发生）
 优点：容易理解，可以绑定多个事件，每个时间可以指定多个回调函数
 缺点：事件驱动型，流程不够清晰
-3.发布、订阅（观察者模式）TODO要求会写＃＃＃＃＃＃
 类似于事件监听，但是可以通过‘消息中心’，了解现在有多少发布者，多少订阅者
-4. Promise对象
 优点：可以利用then方法，进行链 】【【【【【【【【·······················=】式写法；可以书写错误时的回调函数；
 缺点：编写和理解，相对比较难
-5.Generator函数
 优点：函数体内外的数据交换、错误处理机制
 缺点：流程管理不方便
-6.async函数
 优点：内置执行器、更好的语义、更广的适用性、返回的是Promise，结构清晰
 缺点：错误处理机制
```

**js延迟加载的方法有哪些？**

 defer和async、动态创建DOM方式（用的最多），按需异步载入JS

**defer属性：（页面load后执行）**

 script标签定义了defer属性

 用途：表明脚本在执行时不会影响页面的构造。也就是所，脚本会被延迟到整个页面解析完毕之后再执行。

 <script  src=”XXX.js” defer=“defer”</script

**async属性：（页面load前执行）**

 script标签定义了async属性。与defer属性类似，都用于改变处理脚本的行为。同样，只适用于外部脚本文件

 目的：不让页面等待脚本下载和执行，从而异步加载页面其他内容。异步脚本一定会在页面load事件前执行。不能保证脚本会按顺序执行

 <script src=”XXX.js” async</script
defer要等到整个页面在内存中正常渲染结束（DOM 结构完全生成，以及其他脚本执行完成），才会执行；async一旦下载完，渲染引擎就会中断渲染，执行这个脚本以后，再继续渲染。一句话，defer是“渲染完再执行”，async是“下载完就执行”。另外，如果有多个defer脚本，会按照它们在页面出现的顺序加载，而多个async脚本是不能保证加载顺序的。

**动态创建****DOM方式：**

 ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/05A463CC5C6F4C01B62878AC88D46C07/4564](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/05A463CC5C6F4C01B62878AC88D46C07/4564)

 

**数组从小到大排序？**　TODO可以整理下常见的排序方法。思想和代码＃＃＃＃＃＃

 **方法一****:  sort方法**


```
var array = [1, 4, -8, -3, 6, 12, 9, 8];
​      function compare(val1, val2) {
​        return val1 - val2;
​      };
​array.sort(compare);
​document.write(array);
```

**方法二****:冒泡排序**

```
var array = [1, 4, -8, -3, 12, 9];
​    function sort(arr) {
​      for(var i = 0;i < arr.length;i++){
​        ////两两比较,如果前一个比后一个大,则交换位置
​        for(var j = i + 1; j < arr.length; j++) {
​          if(arr[i]  arr[j]) {
​             var temp = arr[i];
​             arr[i] = arr[j];
​             arr[j] = temp;
​          }
​        }
​      }
​    }
sort(array)
console.log(array)
```

 查看其他排序方式可以看:  https://www.cnblogs.com/real-me/p/7103375.html

**求从大到小排序可以先使数组从大到小排序****,然后添加reverse()方法，使数组顺序颠倒**

**为****string扩展一个trim方法,取掉字符串中的所有空格**
```
方法一：trim（）方法------仅能取掉字符串首尾空格
var str = " a b c "
console.log("trim",str.trim());
//trim原理
function Trim(str){
​    return str.replace(/(^\s*)|(\s*$)/g, "");
}
方法二：去除字符中所有的空格
str.replace(/\s/ig,'')
```


**深拷贝和浅拷贝的问题：**TODO

 \1. 深拷贝和浅拷贝值针对Object和Array这样的复杂类型

 \2. a和b指向了同一块内存，所以修改其中任意一个值，另外一个值也会随之变化，这是浅拷贝

 \3. a和b指向同一块内存，但是修改其中任意一个值，另外一个调用的变量，不会受到影响，这是深拷贝

 \4. 浅拷贝:“Object.assign()”方法用于将所有可枚举的属性的值从一个或多个源对象复制到目标对象，它将返回目标对象

 \5. 深拷贝：JSON.parse( )和JSON.stringify( )给了我们一个基本的解决办法。但是函数不能被正确处理

**显示转换与隐式转换**


**显式转换：**主要通过JS定义的数据转换方法TODO

 各种数据类型及其对应的转化规则：

 数据类型          转换为true的值        转换为false的值

 ​     Boolean            true                    false

 ​    String            任何非空字符串         “” (空字符串)

 ​    Number        任何非零数字值(包括无穷大)    0和NaN

 ​    Object           任何对象                  null

 ​    Underfined           n/a                   undefined

**隐式转换：**
是系统默认的，不需要加以声明就可以进行的转换。一般情况下，数据的类型转换通常是由编译系统自动进行的，不需要人工干预

```
大致规则如下：
\1. 对象和布尔值比较
对象和布尔值比较时，对象先转换为字符串，然后再转换为数字，布尔值直接转换为数字
\2. 对象和字符串比较
对象和字符串进行比较时，对象转换为字符串，然后两者进行比较
\3. 对象和数字比较
对象和数字进行比较时，字符串转换为数字，二者再比较
\4. 字符串和数字比较
字符串和数字进行比较时，字符串转换成数字，二者再比较，true=1，false=0
\5. 字符串和布尔值比较
字符串和布尔值进行比较时，二者全部转换成数值再比较
\6. 布尔值和数字比较
布尔值和数字进行比较时，布尔转换为数字，二者比较
```
**父元素和子元素分别有点击事件的情况下****:**

 点击父元素只会触发父元素事件,不会影响到子元素,如果点击子元素,会因为冒泡触发父元素的点击事件,可以阻止默认冒泡事件;
 stoppropagation和cancelBubble的作用是一样的，都是用来阻止浏览器默认的事件冒泡行为其中celBubble是IE提供的方法。


**ForEach和map和for和for..in和for..of的区别在哪里:** TODO


```
相同点：
这两个API都可以遍历数组


不同点：
forEach函数：
是给数组中的每个都执行一遍回调函数,不会返回一个值
Map方法：
是通过调用数组中的每个元素,映射到新元素中,从而返回一个新数组

forEach更多的用来遍历数组 是没有返回值的 
for in 一般常用来遍历对象或json。for...in...返回的是无顺序的key，因此最好不要用来遍历数组
for...of一般用来遍历数组，不能遍历普通的对象，需要通过和Object.keys()搭配使用。可以遍历数组、Set和Map结构、对象，以及字符串还有
某些类似数组的对象
for in循环出的是key，for of循环出的是value
推荐在循环对象属性的时候，使用for...in,在遍历数组的时候的时候使用for...of

遍历对象时的异同：for循环无法用于循环对象，获取不到obj.length; for in 循环遍历对象的属性时，原型链上的所有属性都将被访问，解决方案：使用hasOwnProperty方法过滤或Object.keys会返回自身可枚举属性组成的数组
eg: 
var southSu = {name:'苏南',address:'深圳',age:18,sex:'男',height:176};
for(var i=0;i<southSu.length;i++){
  console.log(typeof i); //空
  console.log(southSu[i]);//空
}


Object.prototype.test = '原型链上的属性,本文由平头哥联盟-首席填坑官∙苏南分享';
 for(var k in southSu){
  console.log(typeof k);//string
  console.log(southSu[k]);// 苏南 , 深圳 , 18 , 男 , 176 ,本文由平头哥联盟-首席填坑官∙苏南分享
}

遍历数组时的异同： for循环 数组下标的typeof类型:number, for in 循环数组下标的typeof类型:string;
eg:
var southSu = ['苏南','深圳','18','男'];
  for(var i=0;i<southSu.length;i++){
  console.log(typeof i); //number
  console.log(southSu[i]);// 苏南 , 深圳 , 18 , 男
}

var arr = ['苏南','深圳','18','男','帅气',"@IT菲酵犯缌?-首席填坑官"];
 for(var k in arr){
 console.log(typeof k);//string
 console.log(arr[k]);// 苏南 , 深圳 , 18 , 男 , 帅气,平头哥联盟-首席填坑官
}
```
**==与===的区别？**

 ===为等同符，当左边与右边的值与类型都完全相等时，会返回true；

 ==为等值符，用来判断值是否相同，不会判断类型是否相同

**addEventListener监听点击事件与click事件有什么区别?**

 addEventListener事件可以对普通元素进行多个事件处理，可以写多个addEventListener事件
 click事件只能使元素运行最新的事件调用，只会创建一个事件函数。

 ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C803E92F19ED48C3AFB76F32C8C9B331/4561](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C803E92F19ED48C3AFB76F32C8C9B331/4561)

 

 ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B9EB58F38724D908E60BF317C48A01A/4568](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B9EB58F38724D908E60BF317C48A01A/4568)

 

**null和undefined的区别?**

```
null用来表示尚未存在的对象
undefined主要指定义了变量，但是并未赋值
NAN （not a Number）不是一个明确数值的数字类型
ECMAScript认为undefined是从null派生出来的，他们的值是一样的，但是类型却不一样。
所以
null == undefined   //true
null === undefined  //false
```

 **JS中定时器有哪些？他们的区别及用法是什么？**

 setTimeout  只执行一次

 setInterval  会一直重复执行


**JS中几种常见的高阶函数**

 高阶函数是对其他函数进行操作的函数，可以将它们作为参数或通过返回它们。简单来说，高阶函数是一个函数，它接收函数作为参数或将函数作为输出返回。

 

**什么是****AJax?为什么使用Ajax?**

 Ajax是一种创建交互网页应用的网页开发技术.

**Ajax包含了一下技术：**

 \1. 基于web标准XHTML+CSS表示

 \2. 使用DOM进行动态显示以及交互

 \3. 使用XML和XSLT进行数据交互及相关操作

 \4. 使用XMLHttpRequest进行一步数据查询、检索；

 \5. 使用Javascript将所有的东西绑定在一起

**简述****ajax的过程。**

 \1. 创建XMLHttpRequest对象,也就是创建一个异步调用对象

 \2. 创建一个新的HTTP请求,并指定该HTTP请求的方法、URL及验证信息

 \3. 设置响应HTTP请求状态变化的函数

 \4. 发送HTTP请求

 \5. 获取异步调用返回的数据

 \6. 使用JavaScript和DOM实现局部刷新

 **Ajax优缺点？**

**Ajax程序的优势在于：**

 通过异步模式，提升了用户体验

 页面无刷新更新（局部更新），用户体验非常好

 Ajax引擎在客户端运行，承担了一部分本来有服务器承担的工作，从而减少了服务负载

 基于标准化的被广发支持的技术，不需要下载插件或小程序

**fetch、ajax、axios之间的详细区别以及优缺点：**
**2. axios**

```
定义：Axios 是一个基于 promise 的 HTTP 库，可以用在浏览器和 node.js 中。
特性：
从浏览器中创建 XMLHttpRequests
从 node.js 创建 http 请求
支持 Promise API
拦截请求和响应  ===axios.interceptors.request.use(callback, errCallback),axios.interceptors.response.use(callback, errCallback)
转换请求数据和响应数据
取消请求  ===使用 cancel token 取消请求
自动转换 JSON 数据
客户端支持防御 XSRF
```

**3. fetch**
 **优缺点：**

```
符合关注分离，没有讲输入、输出和用事件来跟踪的状态混杂在一个对象内
更好更方便的写法
更加底层，提供了丰富的API（request，response）
脱离了XHR，是ES规范里的实现方式
fetch只对网络请求报错，对400/500都当做成功的请求，需要封装去处理
fetch默认不会带cookie，需要添加配置项
fetch不支持abort，不支持超时控制，使用setTimeout以及Promise.reject的实现的超时控制并不能阻止请求过程继续在后台运行，造成了量的浪费
```


**xml和json的区别？**

 1）数据体积方面 ---  JSON相对于XML来讲，数据体积小，传递的速度更快些

 2）数据交互方面 ---  JSON和JS的交互更加方便，更容易解析处理，更好的数据交互

 3）XML对数据描述性比较好

 4）JSON的速度要远远快于XML

 **ES6**

 **列举常用的****ES6特性：**

 \1. let、const

 \2. 箭头函数

 \3. 类的支持

 \4. 字符串模块

 \5. symbols

 \6. Promises


 **箭头函数需要注意哪些地方？**

 当要求动态上下文的时候，就不能够使用箭头函数，也就是this的固定化。

 \1. 没有this，this的指向是定义时所在的对象，而不是使用时所在的对象；

 \2. 不能够用作构造函数，这就是说，不能够使用new命令，否则就会抛出一个错误。

 \3. 不能够使用arguments对象；

 \4. 不能使用yield命令

 箭头函数最直观的三个特点：

 不需要function关键字来创造 匿名函数

 省略return关键字

 修复了this指向
 
**let、const、var**

 ```
 \1. let声明的变量具有块级作用域
 \2. let生命的变量不能通过window.变量名访问
 \3. 形如for(let x...)的循环是每次迭代都为x创建新的绑定
 \4. let约束了变量提升
 \5. let不允许在相同作用域内重复声明同一个变量名，var是允许的
 \6.const定义的常量值，不能够重新赋值，如果值是一个对象，可以改变对象里边的属性值。const变量声明的时候必须初始化
 ```


 **async函数的基本用法:**

 asyn函数返回一个Promise对象，可以使用then方法添加回调函数。当函数执行的时候，一旦遇到await就会先返回，等到异步操作完成，再接着执行函数体内后面的语句。函数前面的async关键字，表明该函数内部有异步操作。调用该函数时，会立即返回一个Promise对象。由于async函数返回的是Promise对象，可以作为await命令的参数。


**async与generator的区别?**

```
async函数是Generator函数的语法糖，async函数就是将Generator函数的星号（*）替换成async，将yield替换成await。
async函数对Generator函数的改进，体现在以下四点：
1、内置执行器
2、更好的语义：async表示函数里有异步操作，await表示紧跟在后面的表达式需要等待结果
3、更广的适用性：async函数的awai他命令后面，可以是Promise对象和原始类型的值（数字、字符串和布尔值，但这时等同于同步操作）
4、返回值是Promise：async函数的返回值是Peomise对象，这比Generator函数的返回值是Iterator对象方便对了，可以用then方法指定下一步的操作。
进一步说，async函数完全可以看作多个异步操作包装成的一个Promise对象，而await命令就是内部then命令的语法糖
```

**有用过****promise吗？请写出下列代码的执行结果，并写出你的理解思路：**TODO
```
setTimeout(()={
​    console.log(1);
}, 0)
 new Promise((resolve)={
​    console.log(2);
​    for(var i = 1; i < 200; i++){
​        i = 198 && resolve()
​    }
​    console.log(3)
}).then(()={
​    console.log(4)
})
console.log(5)// 2 3 5 4 1 

```
解释：
宏任务：[task1,task2,task3…]颗粒度大 实时性不强，要排队
微任务：缩小颗粒度[task1[m1…],task2[m1…],task3[m1…]]，直接插队，实时性强

微任务：在上一个宏任务之后，下一个宏任务之前执行。
第一个 script 标签的代码是第一个宏任务

promise里面是同步，promise.then()是微任务，setTimeout是宏任务。
异步任务大致分为：微任务（micro task，如：promise.then、MutaionObserver等）和宏任务（macro task，如：setTimeout、setInterval、I/O等）。

**Object.is（）与原来的比较操作符===，==的区别？**

```
· ==相等运算符，比较时会自动进行数据类型转换
· ===严格相等运算符，比较时不进行隐式类型转换
· Object.is同值相等算法，在===基础上对0和NaN特别处理
+0 === -0 //true
NaN === NaN // false
Object.is(+0, -0) // false
Object.is(NaN, NaN) // true
```

**字符串模板：**

 ES6中允许使用反引号` 来创建字符串，此方法创建的字符串里面可以包含由${ }包裹的变量


 **解构：**

 自动解析数组或对象中的值。若一个函数要函数要返回多个值，常规的做法是返回一个对象，将每个值作为这个对象的属性返回。在ES6中，利用解构这一特性，可以直接返回一个数组，然后数组中的值会自动被解析到对应接收该值得变量中。


 **参数默认值，不定参数，拓展参数：**

 **默认参数值：**

 可以在定义函数的时候指定参数的默认值，而不用像以前那样通过逻辑或操作符来达到目的了。

```
//传统方式设置默认方式
function sayHello(name){
​    var name = name||'dude';
​    console.log("Hello "+name);
}
sayHello(); //Hello dude
sayHello("wayou"); //Hello wayou


//ES6的默认参数
function sayHello2(name = "dude"){
​    console.log("Hello "+name)
}
sayHello2(); //Hello dude
sayHello2("wayou"); //Hello wayou
```
**不定参数（拓展符）：**

 不定参数是在函数中使用命名参数同时接收不定数量的未命名参数。这只是一种语法糖，在以前的JavaScript代码中我们可以通过arguments变量来达到这一目的。不定参数的格式是三个句点后跟代表所有不定参数的变量名。比如下面这个例子中，...x代表了所有传入add函数的参数。

 <script

 //将所有参数想加的函数

 ```
 function add(...x){

 ​    return x.reduce((m,n)=m+n);
 }

 //传递任意个数的参数

 console.log(add(1,2,3)); //输出:6

 console.log(add(1,2,3,4,5)); //输出:15
 ```

 </script

 reduce（）方法接收一个函数作为累加器，数组中的每个值（从左到右）开始缩减，最终计算为一个值。

 reduce（）可以作为一个高阶函数，用于函数的compose

 注意：reduce（）对于空数组是不会执行回调函数的

 拓展符：将一个数组转为用逗号分隔的参数序列。（若数组为空不产生任何效果）

 <script

 var x = [1,2,3,4,5,6];

 console.log(x); //(6) [1, 2, 3, 4, 5, 6]

 console.log(...x); //1 2 3 4 5 6

 </script

 **拓展参数：**

 拓展参数则是另一种形式的语法糖，它允许传递数组或类数组直接作为函数的参数而不用通过apply。

 <script

 var people = ['wayou','john','sherlock'];

 //sayHello函数来接收三个单独的参数

 function sayHello(people1,people2,people3){

 ​    console.log(`Hello ${people1},${people2},${people3}`)

 }

 //以前的方式,如果需要传递数组当参数,我们需要使用函数apply方法

 sayHello.apply(null,people); //Hello wayou,john,sherlock

 sayHello(...people); //Hello wayou,john,sherlock

 </script

 **iterator/generator:**

 iterator：它是这么一个对象，拥有一个next方法，这个方法返回一个对象{done，value}，这个对象包含两个属性，一个布尔类型的done和包含任意值的value。

 iterable：这是这么一个对象，拥有一个obj[@@iterator]方法，这个方法返回一个iterator

 generator：它是一个特殊的iterator。反的next方法可以接收一个参数并且返回值取决于它的构造函数（generator function）。generator同时拥有一个throw方法。

 generator番薯：即generator的构造函数。此函数内可以使用yield关键字，在yield出现的地方可以通过generator的next或throw方法向外界传递值。generator函数是通过function*来声明的。

 yield关键字：它可以暂停函数的执行，随后可以再进入函数继续执行

 具体详情：https://blog.domenic.me/es6-iterators-generators-and-iterables/

 **模块：**

 在ES6标准中，Javascript原生支持module了。这种将JS代码分割成不同功能的小块进行模块化的概念是在一些三方规范中流行起来的，比如CommonJS和AMD模式。

 将不同功能的代码分别写在不同文件中，各模块只需导出公共接口部分，然后通过模块的导入方式可以在其他地方使用。

**Map、Set和WeakMap、WeakSet** TODO

**Proxies**

 proxy可以监听对象身上发生了什么事情，并在这些事情发生后执行一些相应的操作。一下子让我们对一个对象有了很强的跟踪能力，同时咋数据绑定方面也很有用处。

**修饰器** 来自ES6 +1
定义：是一个函数，用来修改类的行为。
注意：修饰器对类的行为是在代码编译时发生的，而不是在运行时发生的，
修饰器函数的第一个参数就是所要修饰的目标类。
修饰器函数修饰类的函数的时候，第一个参数是所要修饰的目标对象，第二个参数是所要修饰的属性名，第三个参数是该属性的描述对象。
修饰器可以修饰类，类的方法，类的属性。
修饰器不可以修饰函数，因为函数会有变量提升。所以没法修饰函数。
如果有多个修饰器，那么会从外到内进入修饰器，然后从内到外去执行修饰器。
还有一些很多修饰器库,略过......
应用：给类加静态属性，给实例对象加属性和方法(在类的原型上加属性和方法)

**创建自定义对象的方法**
```
1.new Object()
缺点: 要创建多个对象，会产生大量的重复代码。

2.字面量
缺点：要创建多个对象，会产生大量的重复代码。(相同的方法没有得到复用。)

3.工厂模式
function createPerson(name){
  var o = new Object()
  o.name = name;
  o.sayName = function(){
    alert(this.name)
  }
}
缺点：每次调用工厂模式的方式都会返回新的属性和方法。

4.构造函数
function CreatePerson(name) {
  this.name = name
  this.sayName = function(){
    alert(this.name)
  }
}
缺点：方法是不会共享的，每次创建对象都是新的方法。
(1)没有显示的创建对象
(2)直接将属性和方法赋给了this对象
(3)没有return语句

5.原型模式
function Person(){}
Person.prototype.name = 'hare'
Person.prototype.sayName = function(){
  alert(this.name)
}
缺点：原型链上的属性和方法被对象实例所共享
原型中的所有属性是被很多实例所共享的，这种共享对于函数非常合适，对于那些包含基本值的属性倒也说的过去，通过在实例上添加一个同名属性，还可以隐藏原型中的对应属性，然而，对于包含引用类型值的属性来说。就会直接被共享。


6.组合使用构造函数模式和原型模式
function Person(name){
  this.name = name
}
Person.prototype.sayName = function(){
  alert(this.name)
}
特点：实例属性都是在构造函数中定义的，由所有实例共享的属性和方法则在原型中定义

```
**构造函数、原型、实例的关系**
每一个构造函数都有一个原型对象，原型对象都包含一个指向构造函数的指针(constructor),而实例都包含一个指向原型对象的内部指针([[Prototype]])。
**原型链**

**继承**
```
1.原型链
function SuperType() {
 this.colors = ["red", "blue", "green"];
}
function SubType() {}
// 继承 SuperType
SubType.prototype = new SuperType();
let instance1 = new SubType();
instance1.colors.push("black");
console.log(instance1.colors); // "red,blue,green,black"
let instance2 = new SubType();
console.log(instance2.colors); // "red,blue,green,black"
缺点：原型链上的属性和方法被对象实例所共享
如果是简单数据类型会直接在实例上添加一个同名属性，可以直接隐藏原型中的对应属性。

2.借用构造函数
function SuperType() {
 this.colors = ["red", "blue", "green"];
}
function SubType() {
 // 继承 SuperType
 SuperType.call(this);
}
let instance1 = new SubType();
instance1.colors.push("black");
console.log(instance1.colors); // "red,blue,green,black"
let instance2 = new SubType();
console.log(instance2.colors); // "red,blue,green"
缺点：方法都在构造函数中定义，无法函数复用。
优点：解决了原型中包含应用类型值所带来的问题。

3.组合继承
function SuperType(name){
 this.name = name;
 this.colors = ["red", "blue", "green"];
}
SuperType.prototype.sayName = function() {
 console.log(this.name);
};
function SubType(name, age){
 // 继承属性
 SuperType.call(this, name);
 this.age = age;
}
// 继承方法
SubType.prototype = new SuperType();
SubType.prototype.sayAge = function() {
 console.log(this.age);
};
let instance1 = new SubType("Nicholas", 29);
instance1.colors.push("black");
console.log(instance1.colors); // "red,blue,green,black"
instance1.sayName(); // "Nicholas";
instance1.sayAge(); // 29
let instance2 = new SubType("Greg", 27);
console.log(instance2.colors); // "red,blue,green"
instance2.sayName(); // "Greg";
instance2.sayAge(); // 27

优点：通过在原型上定义方法实现了函数复用，又能够保证每个实例都有它自己的属性。

```

**Set**
```
es6提供的新的数据结构，类似数组，没有重复的值。
通过add()方法向 Set 结构加入成员
Set函数可以接受一个数组（或者具有 iterable 接口的其他数据结构）作为参数，用来初始化。

Set 结构的实例有以下属性
Set.prototype.constructor：构造函数，默认就是Set函数。
Set.prototype.size：返回Set实例的成员总数。


Set 实例的方法分为两大类：操作方法（用于操作数据）和遍历方法（用于遍历成员）。
操作方法。

Set.prototype.add(value)：添加某个值，返回 Set 结构本身。
Set.prototype.delete(value)：删除某个值，返回一个布尔值，表示删除是否成功。
Set.prototype.has(value)：返回一个布尔值，表示该值是否为Set的成员。
Set.prototype.clear()：清除所有成员，没有返回值。

Array.from方法可以将 Set 结构转为数组。
Array.from(new Set(array)) //这就提供了去除数组重复成员的另一种方法
[...new Set(array)] //等价

遍历操作
Set 结构的实例有四个遍历方法，可以用于遍历成员。

Set.prototype.keys()：返回键名的遍历器
Set.prototype.values()：返回键值的遍历器
Set.prototype.entries()：返回键值对的遍历器
Set.prototype.forEach()：使用回调函数遍历每个成员

需要特别指出的是，Set的遍历顺序就是插入顺序。这个特性有时非常有用，比如使用 Set 保存一个回调函数列表，调用时就能保证按照添加顺序调用。

扩展运算符（...）内部使用for...of循环，所以也可以用于 Set 结构。

```
**WeakSet**
```
WeakSet 结构与 Set 类似，也是不重复的值的集合。但是，它与 Set 有两个区别。

首先，WeakSet 的成员只能是对象，而不能是其他类型的值。

其次，WeakSet 中的对象都是弱引用
WeakSet 结构有以下三个方法。

WeakSet.prototype.add(value)：向 WeakSet 实例添加一个新成员。
WeakSet.prototype.delete(value)：清除 WeakSet 实例的指定成员。
WeakSet.prototype.has(value)：返回一个布尔值，表示某个值是否在 WeakSet 实例之中。

WeakSet 没有size属性，没有办法遍历它的成员。

WeakSet 不能遍历，是因为成员都是弱引用，随时可能消失，遍历机制无法保证成员的存在，很可能刚刚遍历结束，成员就取不到了。WeakSet 的一个用处，是储存 DOM 节点，而不用担心这些节点从文档移除时，会引发内存泄漏。
```
**Map**
```
size 属性 size属性返回 Map 结构的成员总数。
Map.prototype.set(key, value) set方法设置键名key对应的键值为value，然后返回整个 Map 结构。如果key已经有值，则键值会被更新，否则就新生成该键。
Map.prototype.get(key)  get方法读取key对应的键值，如果找不到key，返回undefined。
Map.prototype.has(key)  has方法返回一个布尔值，表示某个键是否在当前 Map 对象之中。
Map.prototype.delete(key)  delete方法删除某个键，返回true。如果删除失败，返回false。
Map.prototype.clear()  clear方法清除所有成员，没有返回值。

遍历方法
Map 结构原生提供三个遍历器生成函数和一个遍历方法。

Map.prototype.keys()：返回键名的遍历器。
Map.prototype.values()：返回键值的遍历器。
Map.prototype.entries()：返回所有成员的遍历器。
Map.prototype.forEach()：遍历 Map 的所有成员。

```

**与其他数据结构的互相转换 § ⇧**
```
（1）Map 转为数组-- 扩展运算符（...）

[...new Map([
  [true, 7],
  [{foo: 3}, ['abc']]
])]

 （2）数组 转为 Map

new Map([
  [true, 7],
  [{foo: 3}, ['abc']]
])

（3）Map 转为对象 

（4）对象转为 Map
 let map = new Map(Object.entries({"a":1, "b":2}));

（5）Map 转为 JSON
（6）JSON 转为 Map
```

**WeakMap 的语法**

```
WeakMap 与 Map 在 API 上的区别主要是两个，一是没有遍历操作（即没有keys()、values()和entries()方法），也没有size属性。因为没有办法列出所有键名，某个键名是否存在完全不可预测，跟垃圾回收机制是否运行相关。这一刻可以取到键名，下一刻垃圾回收机制突然运行了，这个键名就没了，为了防止出现不确定性，就统一规定不能取到键名。二是无法清空，即不支持clear方法。因此，WeakMap只有四个方法可用：get()、set()、has()、delete()。
```

```
React 并不是完整的 MVC/MVVM 框架，它专注于提供清晰、简洁的 View
（视图）层解决方案。而又与模板引擎不同，React 不仅专注于解决 View 层的问题，又是一个包
括 View 和 Controller 的库。对于复杂的应用，可以根据应用场景自行选择业务层框架，并根据
需要搭配 Flux、Redux、GraphQL/Relay 来使用。
```
