**前端开打掌握的知识内容概要**

**HTML/CSS:** 

对web标准的理解(结构/表现/行为)、浏览器内核、渲染原理、依赖管理、兼容性、CSS语法、层次关系、常用属性、布局、 选择器、权重、盒模型、Hack、CSS预处理器、Flexbox、CSS Modules、Document flow、BFC、HTML5（离线&储存&history、多媒体、webGL、SVG、Cavas）

**Javascript：**

数据类型、运算、对象、function、继承、闭包、  作用域、事件、prototype、RegExp、JSON、Ajax、DOM、BOM、内存泄漏、跨域、异步请求、模板引擎、模块化、Flux、同构、算法、ECMAScript6、Nodejs、HTTP

**其他：**

主流MVVM框架(React\Vue\Angular)、Hybrid App\React Native\Weex、TypeScript、RESTFul、WEB安全、前端工程化、依赖管理、性能优化、重构、团队协作、可维护、易用性、SEO、UED、前端技术选型、快速学习能力等；
>
> 
**JS:**
>
> **JS数据类型有哪些?**
>
> 栈: (原始数据) string/number/boolean/null/undefined/symbol
>
> 堆: (引用数据类型)object(function,Date,Array,正则对象)
>
> 数据类型一共7（6种基本类型+1种引用类型）种
>
**介绍****JS有哪些内置对象？**
>
> object是Javascript中所有对象的父对象
>
> 数据封装类对象：Object、Array、Boolean、Number和String
>
> 其他对象：Function、Arguments、Math、Date、RegExp、Error
>
>**JS几种常见内置对象和方法**
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
>
> 转浮点数parseFloat();
>
> 转字符串toString()/string()
>
> 数组转字符串 join();
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/22E28F5BBF414C7EBFDE3353368BD5E7/4574](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/22E28F5BBF414C7EBFDE3353368BD5E7/4574)
>
> 
>
> 字符串转数组: split();
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C9C4117086614B50AC93D889530D3050/4573](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C9C4117086614B50AC93D889530D3050/4573)
>
> 
>

**栈与堆的区别****?**TODO
>
> 栈与堆的储存位置不同;
>
> 原始数据是储存在栈中简单数据段,体积小,大小固定,属于频繁使用的数据.
>
> 引用数据类型是储存在堆中的对象,占据的空间大,如果储存在栈中会影响运行性能,引用数据类型在栈中指明了自己的所在地.当代码解析时,会先从栈中获取地址,然后再从堆中获取实体;
>
>
**作用域：**
>
>每一个变量、函数都有其作用的范围，超出范围不得使用，这个叫做作用域
>
 **全局变量、局部变量：**
>
> 全局变量：在全局范围内声明的变量，如var a =1；
>
> 只有赋值没有声明的值，如a =1（注：如果a=2在函数环境中，也是全局变量）
>
> 局部变量：写入函数的变量，叫做局部变量，作用范围仅限函数内部
>
> 作用：程序安全，内存的释放
> 

**变量声明提升：**
>
> 在预编译阶段，编译器会把所有定义的变量全部提升到最顶部，即，把变量声明的语句会自动放置在最顶部。
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/D06ED962BAD84E0D9BE5DA09A9B076C9/4575](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/D06ED962BAD84E0D9BE5DA09A9B076C9/4575)
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/03382ACBAF024749ACE39012147C4069/4577](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/03382ACBAF024749ACE39012147C4069/4577)
>
> ​      
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C6131B07D1ED4EA5B4B2A1CFD9A9AF80/4572](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C6131B07D1ED4EA5B4B2A1CFD9A9AF80/4572)
>
> **console.log（a）何时会打印1？**
>
> 当函数内部没有a这个变量的时候，才会向上一级查找
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/CDBBED0684984CD19FFD3D71374C23FE/4578](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/CDBBED0684984CD19FFD3D71374C23FE/4578)
>
> 
>

**作用域链：**
>
> 查找变量的过程。先找自己局部环境内部有没有声明或者是函数，如果有，则查看声明有无赋值或者是函数的内容，如果没有，则向上一级查找。
>

**什么是面向对象编程及面向过程编程，他们的异同和优缺点**
>
> 面向过程就是分析出解决问题所需要的步骤，然后用函数吧这些步骤一步一步实现，使用的时候一个一个一次调用就可以了
>
> 面向对象是把构成问题事务分解成各个对象，建立对象的目的不是为了完成一个步骤，而是为了描述某个事物在整个解决问题的步骤中的行为
>
> 面向对象是以功能来划分问题，而不是步骤
>
**面向对象编程思想**
>
> 基本思想是使用对象、类、继承、封装等基本概念来进行程序设计
>
> 优点：易维护
>
> \- 采用面向对象思想设计的结构，可读性高，由于继承的存在，即使改变需求，那么维护起来是非常方便你和较低成本的
>
> 易扩展
>
> 开发工作的重用性、继承性高、降低重复工作量
>
> 缩短了开发周期
>
**如何解释****this在js中起的作用?**
>
> Js中的this,一般取决于调用这个函数的方法
>
> 1/如果函数被实例化(new 构造函数名())的情况下,this指向全新的对象
>
> 2/如果是某标签触发什么事件,调用了这个函数,this指向标签(整个DOM节点,包含它的子元素);TODO
>
> 3/如果函数使用了call/apply,this是作为参数传入对象
>
> 4/有时候this指向不明确的话,this会指向window,ES6中的箭头函数修改了this指向,永远指向作用域
>
**js中this的用法（经典）：**TODO
>this指向被函数调用的那个对象
> 
☆**说说****JS原型和原型链**
>
**原型**：
>函数都有prototype(显示原型)属性，而prototype会自动初始化一个空对象，这个对象就是原型对象
>
> 原型对象中会有一个constructor属性,这个属性将指向了函数本身
>
> 实例化对象都有一个_proto_(隐式原型)属性，_proto_属性指向原型对象
>
**原型链：**从实例对象往上找构造这个实例的相关对象，然后这个关联的对象再往上找，找到创造它的上一级的原型对象，以此类推，一直到object.prototype原型对象终止,原型链结束.
>
**原型链中的原型对象中的内容****,是会被不同的实例,所共有的**
>
> |      |                                                              |
> | ---- | ------------------------------------------------------------ |
> |      | ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/F684CF201B0846D4A35D835BB9DDA279/4567](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/F684CF201B0846D4A35D835BB9DDA279/4567) |
>
> 
>
**如何准确判断一个变量是数组类型****?**
>
> instanceof用于判断引用类型属于哪个构造函数的方法
>
> var arr = [];
>
> arr  instanceof  Array;  //true
>
> typeof  arr;   //object   typeof是无法判断是否为数组的
>
> **原理****:**
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/4EE1CD020C6949B38C29316A30226C4B/4576](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/4EE1CD020C6949B38C29316A30226C4B/4576)
>
> 
>
> instanceof是用来判断实例的_proto_和构造函数的prototype是否指向一个原型对象，
>
> 但是有一个弊端，只要出现在一条原型链上的，都会返回true（每个函数都有prototype，每个对象都有一个内部属性__proto__，其指向它的原型对象。原型对象也是一个对象，所以也有__proto__）
>
> 这个时候要用实例__proto__.constructor更加严谨
>
> var arr = [ ];
>
> console.log(arr instanseof Array);  //true
>
> console.log(arr.__proto__.constructor === Array)  //true
>
**☆call和apply的区别和作用?**
>
> apply和call都是调用一个对象的一个方法，用另一个对象替换当前对象。
>
> 相同点：方法的含义是一样的，即方法功能是一样的。并且第一个参数的作用是一样的
>
> 不同点：call可以传入多个参数、apply只能传入两个参数，所以其第二个参数往往是作为数组形式传入
>
> 存在意义：实现（多重）继承
>
**继承的方法有哪些？**
>
> 原型链继承、构造继承、实例继承、拷贝继承、组合继承、寄生组合继承
>
**继承详情解释：**
>
> 既然要实现继承，那么我们首先要有一个父类，代码如下:
>
> //先定义一个父类
>
> function Animal(name){
>
> //属性
>
> this.name = name || 'Animal';
>
> //实例方法
>
> this.sleep = function(){
>
> console.log(this.name + "正在睡觉!")
>
> }
>
> }
>
> //原型方法
>
> Animal.prototype.eat = function(food){
>
> console.log(this.name + "正在吃" + food);
>
> }
>
**1.** **原型链继承**
>
**核心：**将父类的实例作为子类的原型
>
> //原型链继承
>
> function Cat(){ }
>
> Cat.prototype = new Animal();
>
> Cat.prototype.name = "cat";
>
> 
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //cat
>
> console.log(cat.eat("fish")); //cat正在吃fish
>
> console.log(cat.sleep()); //cat正在睡觉
>
> console.log(cat instanceof Animal); //true
>
> console.log(cat instanceof Cat); //true
>
**特点：**
>
> \1. 非常纯粹的继承关系，实例是子类的实例，也是父类的实例
>
> \2. 父类新增原型方法、原型属性，子类都能够访问到
>
> \3. 简单，易于实现
>
**缺点：**
>
> \1. 要想实现子类新增属性的方法,必须要在new Animal( )这样的语句之后执行,补鞥呢放在构造器中
>
> \2. 无法实现多继承
>
> \3. 来自原型对象的引用属性是所有实例共享的
>
> \4. 创建子类实例时, 无法向父类构造函数传参
>
**2.** **构造函数**
>
> **核心：**使用父类的构造函数来增强子类实例，等于是赋值父类的实例属性给子类（没用的原型）
>
> //构造函数
>
> function Cat(name){
>
> Animal.call(this);
>
> this.name = name || "Tom"
>
> }
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //Tom
>
> console.log(cat.sleep()); //Tom正在睡觉
>
> console.log(cat instanceof Animal); //false
>
> console.log(cat instanceof Cat); //true
>
**特点：**
>
> \1. 解决了1中，子类实例共享父类引用属性的问题
>
> \2. 创建子类实例时，可以向父类传递参数
>
> \3. 可以实现多继承（call多个父类对象）
>
**缺点：**
>
> \1. 实例并不是父类的实例，只是子类的实例
>
> \2. 只能继承父类的实例属性与方法，不能继承原型属性、方法
>
> \3. 无法实现函数复用，每个子类都有父类实例函数的副本，影响性能
>
**4.** **实例继承**
>
**核心****:** 为父类实例添加新特性，作为子类实例返回
>
> //实例继承
>
> function Cat(name){
>
> var instance = new Animal();
>
> instance.name = name || "Tom";
>
> return instance;
>
> }
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //Tom
>
> console.log(cat.sleep()); //Tom正在睡觉!
>
> console.log(cat instanceof Animal); //true
>
> console.log(cat instanceof Cat); //false
>
**特点：**
>
> \1. 不限制调用方法，不管是new子类（）还是子类（)，返回的对象具有相同的效果
>
**缺点****:**
>
> \1. 实例是父类的实例, 不是子类的实例
>
> \2. 不支持多继承 
>
**4. 拷贝继承**
>
> //拷贝继承
>
> function Cat(name){
>
> var animal = new Animal();
>
> for(var p in animal){
>
> Cat.prototype[p] = animal[p];
>
> }
>
> Cat.prototype.name = name || "Tom"
>
> }
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //Tom
>
> console.log(cat.sleep()); //Tom正在睡觉!
>
> console.log(cat instanceof Animal); //false
>
> console.log(cat instanceof Cat); //true
>
**特点：**
>
> \1. 支持多继承
>
**缺点：**
>
> \1. 效率较低，内存占用高（因为要拷贝父类的属性）
>
> \2. 无法获取父类不可枚举的方法（不可枚举方法，不能使用for in 访问到）
>
**5.组合继承**
>
**核心：**通过调用父类构造，继承父类的属性并保留传参的优点，然后通过将父类实例作为子类原型，实现函数复用
>
> //组合继承
>
> function Cat(name){
>
> Animal.call(this);
>
> this.name = name || "Tom";
>
> }
>
> Cat.prototype = new Animal();
>
> //组合继承也需要修复构造函数的指向问题
>
> Cat.prototype.constructor = Cat;
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //Tom
>
> console.log(cat.sleep()); //Tom正在睡觉!
>
> console.log(cat instanceof Animal); //true
>
> console.log(cat instanceof Cat); //true
>
 **特点：**
>
> \1. 弥补了方法2的缺陷，可以继承实例属性、方法，也可以继承原型属性和方法
>
> \2. 既是子类的实例，也是父类的实例
>
> \3. 不存在引用属性共享的问题
>
> \4. 可传参
>
> \5. 函数可复用
>
**缺点：**
>
> \1. 调用了两次父类构造函数，生成了两份实例（子类实例将子类原型上的那份屏蔽了）
>
 **6.  寄生组合继承**
>
> **核心：**通过寄生方式，砍掉父类的实例属性，这样，在调用两次父类的构造的时候，就不会初始化两次实例方法、属性，避免了组合继承的缺点
>
> //寄生组合继承
>
> function Cat(name){
>
> Animal.call(this);
>
> this.name = name || "Tom"
>
> }
>
> (function(){
>
> //创建一个没有实例方法的类
>
> var Super = function(){};
>
> Super.prototype = Animal.prototype;
>
> //将实例作为子类的原型
>
> Cat.prototype = new Super();
>
> })();
>
> //Test Code
>
> var cat = new Cat();
>
> console.log(cat.name); //Tom
>
> console.log(cat.sleep()); //Tom正在睡觉!
>
> console.log(cat instanceof Animal); //true
>
> console.log(cat instanceof Cat); //true
>
> //该实现没有修复constructoe
>
> **特点****:**
>
> \1. 堪称完美
>
> **缺点****:**
>
> \1. 实现较为复杂
>
**☆什么是闭包？闭包有什么作用？**
>
> 由于在js中，变量到的作用域属于函数作用域，在函数执行后作用域会被清除、内存也会随之被回收，但是由于闭包是建立在一个函数内部的子函数，由于其可访问上级作用域的原因，即使上级函数执行完，作用域也不会随之销毁，这时的子函数---也就是闭包，便拥有了访问上级作用域中的变量权限，即使上级函数执行完后，作用域内的值也不会被销毁。
>
> 闭包解决了什么：在本质上，闭包就是将函数内部和函数外部连接起来的一座桥梁。
>
> 由于闭包可以缓存上级作用域，那么就使得函数外部打破了“函数作用域”的束缚，可以访问函数内部的变量。以平时使用的Ajax成功回调为例，这里其实就是个闭包，由于上述的特性，回调就拥有了整个上级作用域的访问和操作能力，提高了几大的便利。开发者不用去写钩子函数来操作审计函数作用域内部的变量了。
>
> 闭包有哪些应用场景：
>
> 闭包随处可见，一个Ajax请求的成功回调，一个事件绑定的回调函数，一个setTimeout的延时回调，或者一个函数内部返回另一个匿名函数，这些都是闭包。简而言之，无论使用何种方式对函数类型的值进行传递，当函数在别处被调用时都有闭包的身影
>
> 闭包的缺陷：由于闭包打破了函数作用域的束缚，导致里面的数据无法清除销毁，当数据过大时会导致数据溢出
>
**事件代理（事件委托）****:**TODO
>
> 事件代理是将子元素的事件写一个父元素,让父元素代替处理,内部使用e.target,e.target就是触发这个事件的子元素
>
**事件的各个阶段**
>
> 捕获阶段  --->  目标阶段  --->  冒泡阶段
>
> document  --->  target目标  --->  document
>
> 由此addEventListener的第三个参数设置为true和false的区别已经非常清晰了
>
> true--->代表该元素在事件的”捕获阶段”(由外向内传递)响应事件
>
> false --->表示该元素在事件的”冒泡阶段”(由内向外传递)响应事件
>
**☆new操作符在创建实例的时候经历了哪几个阶段**TODO
>
> new创建了一个对象，共经历了4个阶段：
>
> \1. 创建一个空对象
>
> \2. 设置原型链
>
> \3. 让实例化对象中的this指向对象，并执行函数体
>
> \4. 判断实例化对象的返回值类型
>
**异步编程的实现方式**
>
> -回调函数
>
> 优点：简单、容易理解
>
> 缺点：不利于维护，代码耦合高
>
> -事件监听（采用时间驱动模式，取决于某个事件是否发生）
>
> 优点：容易理解，可以绑定多个事件，每个时间可以指定多个回调函数
>
> 缺点：事件驱动型，流程不够清晰
>
> -发布、订阅（观察者模式）
>
> 类似于事件监听，但是可以通过‘消息中心’，了解现在有多少发布者，多少订阅者
>
> \- Promise对象
>
> 优点：可以利用then方法，进行链式写法；可以书写错误时的回调函数；
>
> 缺点：编写和理解，相对比较难
>
> -Generator函数
>
> 优点：函数体内外的数据交换、错误处理机制
>
> 缺点：流程管理不方便
>
> -async函数
>
> 优点：内置执行器、更好的语义、更广的适用性、返回的是Promise，结构清晰
>
> 缺点：错误处理机制
>
**对原生****JS了解程度**
>
> 数据类型、运算、对象、Function、继承、闭包、作用域、原型链、事件、RegExp、JSON、Ajax、DOM、BOM、内存泄漏、跨域、异步装载、模板引擎、前端MVC、MVVM、路由、模块华、Canvas、ECMAScript
>
> 
>
**js延迟加载的方法有哪些？**
>
> defer和async、动态创建DOM方式（用的最多），按需异步载入JS
>
**defer属性：（页面load后执行）**
>
> script标签定义了defer属性
>
> 用途：表明脚本在执行时不会影响页面的构造。也就是所，脚本会被延迟到整个页面解析完毕之后再执行。
>
> <script  src=”XXX.js” defer=“defer”></script>
>
**async属性：（页面load前执行）**
>
> script标签定义了async属性。与defer属性类似，都用于改变处理脚本的行为。同样，只适用于外部脚本文件
>
> 目的：不让页面等待脚本下载和执行，从而异步加载页面其他内容。异步脚本一定会在页面load事件前执行。不能保证脚本会按顺序执行
>
> <script src=”XXX.js” async></script>
>
**动态创建****DOM方式：**
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/05A463CC5C6F4C01B62878AC88D46C07/4564](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/05A463CC5C6F4C01B62878AC88D46C07/4564)
>
> 
>
**数组从小到大排序？**
>
> **方法一****:  sort方法**
>
> var array = [1, 4, -8, -3, 6, 12, 9, 8];
>
> ​      function compare(val1, val2) {
>
> ​        return val1 - val2;
>
> ​      };
>
> ​      array.sort(compare);
>
> ​      document.write(array);
>
**方法二****:冒泡排序**
>
> var array = [1, 4, -8, -3, 12, 9];
>
> ​    function sort(arr) {
>
> ​      for(var i = 0;i < arr.length;i++){
>
> ​        ////两两比较,如果前一个比后一个大,则交换位置
>
> ​        for(var j = i + 1; j < arr.length; j++) {
>
> ​          if(arr[i] > arr[j]) {
>
> ​             var temp = arr[i];
>
> ​             arr[i] = arr[j];
>
> ​             arr[j] = temp;
>
> ​          }
>
> ​        }
>
> ​      }
>
> ​    }
>
> sort(array);
>
> console.log(array)
>
> 查看其他排序方式可以看:  https://www.cnblogs.com/real-me/p/7103375.html
>
**求从大到小排序可以先使数组从大到小排序****,然后添加reverse()方法，使数组顺序颠倒**
>
**为****string扩展一个trim方法,取掉字符串中的所有空格**
>
> 方法一：trim（）方法------仅能取掉字符串首尾空格
>
> var str = " a b c "
>
> console.log("trim",str.trim());
>
> //trim原理
>
> function Trim(str){
>
> ​    return str.replace(/(^\s*)|(\s*$)/g, "");
>
> }
>
> 方法二：去除字符中所有的空格
>
> str.replace(/\s/ig,'')
>
> 
>
**如何实现数组的随机排序****?**
>
> 最快是给数组添加原生sort()方法,可以随机数组,如果sort(),方法没有参数的话,就是依照数据的unicode ['junɪˌkod]码排序的
>
> 可以在sort()中添加一个比较函数函数:
>
> function(a,b){  return Math.rendom()>.5? -1:1  }
>
> Math.rendom()在0到1之间生成一个随机数
>
**图片懒加载**
>
**图片懒加载理解：**由于商城图片过多时，就会给图片加一个懒加载的缓冲效果。当图片进入可视化区域的时候才会加载，否则图片只是一个空标签。这样可以优化页面渲染速度，提升用户体验。
>
**思路：**将页面中的所有img属性src用data-src代替，当页面滚动至此图片出现在可视区域时，用js取到该图片的data-src值赋给src。
>
> 
>
**所用知识点：**
>
> 浏览器可视区域的宽高：
>
> js :   document.body.clientWidth/clientHeight
>
> jquery:  var windHeight = $(window).width()/$(window).height();
>
> 获取滚动条相对于顶部的高度:
>
> js :  document.body.scrollTop;
>
> jquery :  var  scrollTop=$(window).scrollTop;
>
> 获得元素对于浏览器顶部的高度:
>
> js :  DOM元素.offsetTop;
>
> jquery:  var imgTop=$('img').offset().top
>
> 判断元素是否出现在浏览器的可视化区域内:
>
> 元素相对于顶部的高度 - 浏览器可视化区域的高度 < 小于滚动条到顶部的高度  
>
> 成立就代表出现 : 不成立就没出现
>
> 怎样排除首屏的图片
>
> 元素到顶部距离 - 浏览器的可视化高度  >  0
>
> 排除已加载的图片
>
> $(this).attr(‘src’) != $(this).attr(‘data-src’)  //排除已加载的图片
>
**Jquery实现图片懒加载 :**
>
> <script>
>
> // 注意: 需要引入jQuery和underscore
>
> $(function() {
>
> ​     // 获取window的引用:
>
> ​     var $window = $(window);
>
> ​     // 获取包含data-src属性的img，并以jQuery对象存入数组:
>
> ​     var lazyImgs = _.map($('img[data-src]').get(), function (i) {
>
> ​       return $(i);
>
> ​     });
>
> ​     // 定义事件函数:
>
> ​     var onScroll = function() {
>
> ​       // 获取页面滚动的高度:
>
> ​       var wtop = $window.scrollTop();
>
> ​       // 判断是否还有未加载的img:
>
> ​       if (lazyImgs.length > 0) {
>
> ​         // 获取可视区域高度:
>
> ​         var wheight = $window.height();
>
> ​         // 存放待删除的索引:
>
> ​         var loadedIndex = [];
>
> ​         // 循环处理数组的每个img元素:
>
> ​         _.each(lazyImgs, function ($i, index) {
>
> ​           // 判断是否在可视范围内:
>
> ​           if ($i.offset().top - wtop < wheight) {
>
> ​             // 设置src属性:
>
> ​             $i.attr('src', $i.attr('data-src'));
>
> ​             // 添加到待删除数组:
>
> ​             loadedIndex.unshift(index);
>
> ​           }
>
> ​         });
>
> ​         // 删除已处理的对象:
>
> ​         _.each(loadedIndex, function (index) {
>
> ​           lazyImgs.splice(index, 1);
>
> ​         });
>
> ​       }
>
> ​     };
>
> ​     // 绑定事件:
>
> ​     $window.scroll(onScroll);
>
> ​     // 手动触发一次:
>
> ​     onScroll();
>
> </script>
>
> onScroll()函数最后要手动触发一次，因为页面显示时，并未触发scroll事件。如果图片已经在可视化区域内，这些图片仍然是loading状态，需要手动触发一次，就可以正常显示。
>
**js中常见的内存泄漏：**
>
> \1. 内存泄漏会导致一系列问题，比如：运行缓慢、崩溃、高延迟
>
> \2. 内存泄漏是指你用不到（访问不到）的变量，依然占据着内存空间，不能被再次利用起来
>
> \3. 意外的全局变量，这些都是不会被回收的变量（除非设置null或者被重新赋值），特别是那些用来临时存储大量信息的变量
>
> \4. 周期函数一直在运行，处理函数并不会被回收，jq在移除节点前都会，将事件监听移除
>
> \5. js代码中有对DOM节点的引用，dom节点被移除的时候，引用还维持
>
**深拷贝和浅拷贝的问题：**TODO
>
> \1. 深拷贝和浅拷贝值针对Object和Array这样的复杂类型
>
> \2. a和b指向了同一块内存，所以修改其中任意一个值，另外一个值也会随之变化，这是浅拷贝
>
> \3. a和b指向同一块内存，但是修改其中任意一个值，另外一个调用的变量，不会受到影响，这是深拷贝
>
> \4. 浅拷贝:“Object.assign()”方法用于将所有可枚举的属性的值从一个或多个源对象复制到目标对象，它将返回目标对象
>
> \5. 深拷贝：JSON.parse( )和JSON.stringify( )给了我们一个基本的解决办法。但是函数不能被正确处理
>
**显示转换与隐式转换**
>
> JS中有5中简单的数据类型（也称之为基本数据类型）：undefined、Null、Boolean、Number、String。还有一种复杂的数据--------Object，Object本质是一组无序的名值对组成的。
>
> 对一个值使用typeof操作符可以返回该值的数据类型，typeof操作符会返回一些令人迷惑但技术上却正确的值，比如调用typeof null会返回“object”，应为特殊值null被认为是一个空的对象引用。
>
**显式转换：**主要通过JS定义的数据转换方法TODO
>
> 各种数据类型及其对应的转化规则：
>
> 数据类型          转换为true的值        转换为false的值
>
> ​     Boolean            true                    false
>
> ​    String            任何非空字符串         “” (空字符串)
>
> ​    Number        任何非零数字值(包括无穷大)    0和NaN
>
> ​    Object           任何对象                  null
>
> ​    Underfined           n/a                   undefined
>
**隐式转换：**是系统默认的，不需要加以声明就可以进行的转换。一般情况下，数据的类型转换通常是由编译系统自动进行的，不需要人工干预
>
> 大致规则如下：
>
> \1. 对象和布尔值比较
>
> 对象和布尔值比较时，对象先转换为字符串，然后再转换为数字，布尔值直接转换为数字
>
> \2. 对象和字符串比较
>
> 对象和字符串进行比较时，对象转换为字符串，然后两者进行比较
>
> \3. 对象和数字比较
>
> 对象和数字进行比较时，字符串转换为数字，二者再比较
>
> \4. 字符串和数字比较
>
> 字符串和数字进行比较时，字符串转换成数字，二者再比较，true=1，false=0
>
> \5. 字符串和布尔值比较
>
> 字符串和布尔值进行比较时，二者全部转换成数值再比较
>
> \6. 布尔值和数字比较
>
> 布尔值和数字进行比较时，布尔转换为数字，二者比较
>
**父元素和子元素分别有点击事件的情况下****:**
>
> 点击父元素只会触发父元素事件,不会影响到子元素,如果点击子元素,会因为冒泡触发父元素的点击事件,可是阻止默认冒泡事件;
>
**mouseover/mouseout与mouseenter/mouseleave的区别与联系**
>
> \1. mouseover/mouseout是标准事件，所有浏览器都支持；mouseenter/mouseleave是IE5.5引入的特有事件,后来被DOM3标准采纳，现代浏览器也支持
>
> mouseover/mouseout是冒泡事件;mouseenter/mouseleave不冒泡.需要为多个元素监听鼠标移入/移出事件时，推荐使用mouseover、mouseout托管，提高性能
>
> 
>
**ForEach和map的区别在哪里:**
>
> 这两个API都可以遍历数组
>
> forEach函数,是给数组中的每个都执行一遍回调函数,不会返回一个值
>
> |      |                                                              |
> | ---- | ------------------------------------------------------------ |
> |      | ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/958C476FC7BD4E07A95503383DB6E134/4566](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/958C476FC7BD4E07A95503383DB6E134/4566) |
>
> Map方法是通过调用数组中的每个元素,映射到新元素中,从而返回一个新数组
>
> 如果是复合型类型时，如果只改变复合类型的其中某个value时，将可以正常使用
>
**JS判断设备来源**
>
**function** **deviceType**(){
>
> ​    **var** ua = navigator.userAgent;
>
> ​    **var** agent = ["Android", "iPhone", "SymbianOS", "Windows Phone", "iPad", "iPod"];   
>
> ​    **for**(**var** i=0; i<len,len = agent.length; i++){
>
> ​      **if**(ua.indexOf(agent[i])>0){     
>
> ​        **break**;
>
> ​      }
>
> ​    }
>
> }
>
> deviceType();
>
> window.addEventListener('resize', **function**(){
>
> ​    deviceType();
>
> })
>
> //微信的 有些不太一样
>
> **function** **isWeixin**(){
>
> ​    **var** ua = navigator.userAgent.toLowerCase();
>
> ​    **if**(ua.match(/MicroMessenger/i)=='micromessenger'){
>
> ​      **return** true;
>
> ​    }**else**{
>
> ​      **return** false;
>
> ​    }
>
> }
>
**DOM元素的e的e.getAttribute(propName)和e.propName有什么区别和联系?**TODO
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
**==与===的区别？**
>
> ===为等同符，当左边与右边的值与类型都完全相等时，会返回true；
>
> ==为等值符，用来判断值是否相同，不会判断类型是否相同
>
**addEventListener监听点击事件与click事件有什么区别?**
>
> addEventListener事件可以对普通元素进行多个事件处理，click事件只能使元素运行最新的事件结果
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C803E92F19ED48C3AFB76F32C8C9B331/4561](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/C803E92F19ED48C3AFB76F32C8C9B331/4561)
>
> 
>
> ![https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B9EB58F38724D908E60BF317C48A01A/4568](https://note.youdao.com/yws/public/resource/b1780c5a1dfb87d402449badc06922b2/xmlnote/5B9EB58F38724D908E60BF317C48A01A/4568)
>
> 
>
**null和undefined的区别?**
>
> null用来表示尚未存在的对象，常用来表示函数企图返回一个不存在对象
>
> undefined主要指定义了变量，但是并未赋值
>
> NAN （not a Number）不是一个明确数值的数字类型
>
> ECMAScript认为undefined是从null派生出来的，他们的值是一样的，但是类型却不一样。
>
> 所以
>
> null == undefined   //true
>
> null === undefined  //false
>
**字符串操作方法。**
>

>

>
**js的 for 跟for in 循环它们之间的区别？**
>
> · 遍历数组时的异同： for循环 数组下标的typeof类型:number, for in 循环数组下标的typeof类型:string;
>
> **var** southSu = ['苏南','深圳','18','男'];**for**(**var** i=0;i<southSu.length;i++){
>
> console.log(**typeof** i); //number
>
> console.log(southSu[i]);// 苏南 , 深圳 , 18 , 男
>
> }**var** arr = ['苏南','深圳','18','男','帅气',"@IT菲酵犯缌?-首席填坑官"];**for**(**var** k **in** arr){
>
> console.log(**typeof** k);//string
>
> console.log(arr[k]);// 苏南 , 深圳 , 18 , 男 , 帅气,平头哥联盟-首席填坑官
>
> }
>
> · 遍历对象时的异同：for循环 无法用于循环对象，获取不到obj.length; for in 循环遍历对象的属性时，原型链上的所有属性都将被访问，解决方案：使用hasOwnProperty方法过滤或Object.keys会返回自身可枚举属性组成的数组
>
> Object.prototype.test = '原型链上的属性,本文由平头哥联盟-首席填坑官∙苏南分享';**var** southSu = {name:'苏南',address:'深圳',age:18,sex:'男',height:176};**for**(**var** i=0;i<southSu.length;i++){
>
> console.log(**typeof** i); //空
>
> console.log(southSu[i]);//空
>
> }
>
> 
>
> **for**(**var** k **in** southSu){
>
> console.log(**typeof** k);//string
>
> console.log(southSu[k]);// 苏南 , 深圳 , 18 , 男 , 176 ,本文由平头哥联盟-首席填坑官∙苏南分享
>
> }
>
> **push()****、****pop()****、****shift()****、****unshift()分别是什么功能？**
>
> push 方法 将新元素添加到一个数组中，并返回数组的新长度值。
>
> var a=[1,2,3,4]; a.push(5);
>
> pop 方法 移除数组中的最后一个元素并返回该元素。
>
> var a=[1,2,3,4]; a.pop();
>
> shift 方法 移除数组中的第一个元素并返回该元素。
>
> var a=[1,2]; alert(a.shift());
>
> unshift 方法 将指定的元素插入数组开始位置并返回该数组。
>
> **如果用原生****js给一个按钮绑定两个click事件？**
>
> 使用事件监听，可给一个DOM节点绑定多个事件（addEventListener）
>
> **拖拽会用到哪些事件？**
>
> dragstart---拖拽开始时在被拖拽元素上触发此事件，监听器需要设置拖拽所需数据，操作系统拖拽文件到浏览器时不触发此事件
>
> dragenter---拖拽鼠标进入元素时在该元素上触发，用于给拖放的元素设置视觉反馈，如高亮
>
> dragover---拖拽时鼠标在目标元素上移动时触发，监听器通过组织浏览器默认行为设置元素为可拖放元素
>
> dragleave---拖拽时鼠标移出目标元素时在目标元素上触发，此时监听器可以取消掉前面设置的视觉效果
>
> drag---拖拽期间在被拖拽元素上连续触发
>
> drop---鼠标在拖放目标上释放时，在拖放目标上触发，此时监听器需要收集数据并且执行所需操作，如果是从操作系统拖放文件到浏览器，需要取消浏览器默认行为
>
> dragend---鼠标在拖放目标上释放时，在拖拽元素上触发，将元素从浏览器拖放到操作系统时不会触发此事件
>
> **JS中定时器有哪些？他们的区别及用法是什么？**
>
> setTimeout  只执行一次
>
> setInterval  会一直重复执行
>
> **document.write和innerHTML的区别?**
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
>
**JS中几种常见的高阶函数**
>
> 高阶函数是对其他函数进行操作的函数，可以将它们作为参数或通过返回它们。简单来说，高阶函数是一个函数，它接收函数作为参数或将函数作为输出返回。
>
> 
>

**什么是****AJax?为什么使用Ajax?**
>
> Ajax是一种创建交互网页应用的网页开发技术.
>
**Ajax包含了一下技术：**
>
> \1. 基于web标准XHTML+CSS表示
>
> \2. 使用DOM进行动态显示以及交互
>
> \3. 使用XML和XSLT进行数据交互及相关操作
>
> \4. 使用XMLHttpRequest进行一步数据查询、检索；
>
> \5. 使用Javascript将所有的东西绑定在一起
>
**简述****ajax的过程。**
>
> \1. 创建XMLHttpRequest对象,也就是创建一个异步调用对象
>
> \2. 创建一个新的HTTP请求,并指定该HTTP请求的方法、URL及验证信息
>
> \3. 设置响应HTTP请求状态变化的函数
>
> \4. 发送HTTP请求
>
> \5. 获取异步调用返回的数据
>
> \6. 使用JavaScript和DOM实现局部刷新
>
> **Ajax优缺点？**
>
**Ajax程序的优势在于：**
>
> 通过异步模式，提升了用户体验
>
> 页面无刷新更新（局部更新），用户体验非常好
>
> Ajax引擎在客户端运行，承担了一部分本来有服务器承担的工作，从而减少了服务负载
>
> 基于标准化的被广发支持的技术，不需要下载插件或小程序
>
**Ajax的缺点：**
>
> Ajax不支持浏览器back按钮
>
> 安全问题，Ajax暴露了与服务器交互的细节
>
> 对搜索引擎的支持比较弱
>
> 破坏了程序的异常机制
>
> 不容易调试
>
**XMLHttpRequest通用属性和方法**
>
> \1. readyState：表示请求状态的整数、取值：
>
> UNSENT(0) : 对象已创建
>
> OPENED(1) : open( )成功调用，在这个状态下，可以xhr设置请求头，或者使用send（）发送请求
>
> HEADERS——RECEIVED(2) : 所有重定向已经自动完成访问，并且最终响应的HTTP头已经收到
>
> LOADING(3) : 响应体正在接收
>
> DONE(4) : 数据传输完成或者传输产生错误
>
> \2. onreadystatechange : readyState改变时调用的函数
>
> \3. status : 服务器返回的HTTP状态码 (如 : 200、404)
>
> \4. statusText : 服务器返回的HTTP状态信息 (如 : OK、No Content)
>
> \5. responseText：作为字符串形式的来自服务器的完整响应式
>
> \6. responseXML：Document对象，表示服务器的响应解析成的XML文档
>
> \7. abort(): 取消异步HTTP请求
>
> \8. getAllResponseHeaders() : 返回一个字符串,包含响应中服务器发送的全部HTTP包头。每个报头都是一个用冒号分割名、值对，并且使用一个回车、换行来分割报头行
>
> \9. getResponseHeader（headerName）：返回haedName对应的报头值
>
> \10. open（method，url，asynchronous，[user，password]）：初始化准备发送到服务器上的请求。method是HTTP方法，不区分大小写；url是请求发送的相对或绝对URL；asynchronous表示请求是否异步；user和password提供身份验证
>
> \11. setRequestHeader（name，value）：设置HTTP报头
>
> \12. send（body）：对服务器进行初始化。参数body包含请求的主体部分，对于POST请求为键值对字符串；对于GET请求，为null
>

> 原生实现:
>
> **var** script = document.createElement('script');
>
> ​      script.type = 'text/javascript';
>
> ​      // 传参并指定回调执行函数为onBack
>
> ​      script.src = 'http://www.....:8080/login?user=admin&callback=onBack';
>
> ​      document.head.appendChild(script);
>
> ​    
>
> ​      // 回调执行函数
>
> ​      **function** **onBack**(res) {
>
> ​        alert(JSON.stringify(res));
>
> ​      }
>
> \2. document.domain+iframe跨域
>
> 此方案仅限主域相同,子域不同的跨域应用场景
>
> 1>父窗口:(http://www.domain.com/a.html)
>
> <iframe id="iframe" src="http://child.domain.com/b.html"></iframe>
>
>             <script>
>
> ​        document.domain = 'domain.com';
>
> ​        **var** user = 'admin';
>
> ​      </script>
>
> 2>子窗口(http://child.domain.com/b.html)
>
>   <script>
>
> ​        document.domain = 'domain.com';
>
> ​        // 获取父窗口中变量
>
> ​        alert('get js data from parent ---> ' + window.parent.user);
>
> ​      </script>
>
> 弊端:查看页面渲染优化
>
> \3. nginx代理跨域
>
> \4. nodejs中间件代理跨域
>
> \5. 后端在头部信息里面设置安全域名
>
> 
**fetch、ajax、axios之间的详细区别以及优缺点：**
>
> \1. JQuery ajax
>
> //JQuery ajax
>
> $.ajax({
>
> type: "POST",
>
> url: url,
>
> data: data,
>
> dataType: dataType,
>
> success: function(){},
>
> error: function(){}
>
> })
>
> **优缺点：**
>
> 本身针对MVC的编程，不符合现在前端MVVM的浪潮
>
> 基于原生的XHR开发，XHR本身的架构不清晰，已经有了fetch的替代方案
>
> JQuery整个项目太大，单纯使用ajax却要引入整个JQuery非常不合理（采取个性打包的方案又不能享受CDN服务）
>
**2. axios**
>
>
> axios({
>
> methods: "post",
>
> url: url,
>
> data:{
>
> data_key: data_value,
>
> ...
>
> }
>
> })
>
> .then(function(response){
>
> console.log(response)
>
> })
>
> .catch(function(error){
>
> console.log(error)
>
> })
>
> **优缺点：**
>
> 从node.js创建http请求
>
> 支持Promise API
>
> 客户端支持防止CSRF
>
> 提供了一些并发请求的接口（重要，方便了很多的操作）
>
**3. fetch**
> try{
>
> let response = await fetch(url);
>
> let data = response.json();
>
> }catch(e){
>
> console.log("Oops,error",e)
>
> }
>
> **优缺点：**
>
> 符合关注分离，没有讲输入、输出和用事件来跟踪的状态混杂在一个对象内
>
> 更好更方便的写法
>
> 更加底层，提供了丰富的API（request，response）
>
> 脱离了XHR，是ES规范里的实现方式
>
> fetch只对网络请求报错，对400/500都当做成功的请求，需要封装去处理
>
> fetch默认不会带cookie，需要添加配置项
>
> fetch不支持abort，不支持超时控制，使用setTimeout以及Promise.reject的实现的超时控制并不能阻止请求过程继续在后台运行，造成了量的浪费
>
**为什么要用****axios？**
>
> axios是一个基于Promise用于浏览器和nodejs的HTTP客户端，本身具有以下特点
>
> 从浏览器中创建XMLHttpRequest
>
> 从nodejs发出http请求
>
> 支持Promise API
>
> 拦截请求和响应
>
> 转换请求和响应数据
>
> 取消请求
>
> 自动转换JSON数据
>
> 客户端支持防止CSRF、XSRF
>
**axios是什么？怎么使用？描述使用它实现登录功能的流程？**
>
> 请求后台资源的模块。使用npm install axios -S安装
>
> 然后发送的事跨域。需要在配置文件中config/index.js进行设置。
>
> 后台如果是TP5则定义一个资源路由。js中使用import进行设置，然后.get或.post。成功返回在.then函数中，失败返回.catch函数中
>
**xml和json的区别？**
>
> 1）数据体积方面 ---  JSON相对于XML来讲，数据体积小，传递的速度更快些
>
> 2）数据交互方面 ---  JSON和JS的交互更加方便，更容易解析处理，更好的数据交互
>
> 3）XML对数据描述性比较好
>
> 4）JSON的速度要远远快于XML
>
> **ES6**
>
> **列举常用的****ES6特性：**
>
> \1. let、const
>
> \2. 箭头函数
>
> \3. 类的支持
>
> \4. 字符串模块
>
> \5. symbols
>
> \6. Promises
>
>
> **箭头函数需要注意哪些地方？**
>
> 当要求动态上下文的时候，就不能够使用箭头函数，也就是this的固定化。
>
> \1. 在使用=>定义函数的时候，this的指向是定义时所在的对象，而不是使用时所在的对象；
>
> \2. 不能够用作构造函数，这就是说，不能够使用new命令，否则就会抛出一个错误。
>
> \3. 不能够使用arguments对象；
>
> \4. 不能使用yield命令
>
> 箭头函数是函数的一种简写形式，使用括号包裹参数，跟随一个=>，紧接着是函数体
>
> 箭头函数最直观的三个特点：
>
> 不需要function关键字来创造
>
> 省略return关键字
>
> 修复了this指向
**let、const、var**
>
> var声明变量的作用域限制在其声明位置的上下文中，而非声明变量总是全局的
>
> 由于变量声明（以及其他声明）总是在任意代码执行之前处理的，所以在代码中的任意位置声明变量总是等效于在代码开头声明；
>
> let是更完美的var，不是全局变量，具有块级函数作用域，大多数情况不会发生变量提升。
>
> \1. let声明的变量具有块级作用域
>
> \2. let生命的变量不能通过window.变量名访问
>
> \3. 形如for(let x...)的循环是每次迭代都为x创建新的绑定
>
> \4. let约束了变量提升
>
> \5. let不允许在相同作用域内重复声明同一个变量名，var是允许的
>
> const定义的常量值，不能够重新赋值，如果值是一个对象，可以改变对象里边的属性值。const变量声明的时候必须初始化
>

**Set数据结构**TODO
>
> ES6中的Set方法本身是一个构造函数，它类似于数组，但是成员的值都是唯一的
>
**拓展：数组去重的方法**
>
> ES6 set方法
>
> var arr = new Set([1,2,2,3,4]);
>
> console.log([...arr]); //(4) [1, 2, 3, 4]
>
> 以往去重方法
>
> var arr = [1,1,2,2,3,4];
>
> //创建一个空数组用于接收不重复内容的数组
>
> var new_arr = [];
>
> for(var i = 0;i<arr.length;i++){
>
> ​    if(new_arr.indexOf(arr[i])==-1){ //判断arr[i]在new_arr中是否存在相同的内容,不存在则push到数组中
>
> ​      new_arr.push(arr[i])
>
> ​    }
>
> }
>
> console.log(new_arr); //(4) [1, 2, 3, 4]
>
>

 **async函数的基本用法:**
>
> asyn函数返回一个Promise对象，可以使用then方法添加回调函数。当函数执行的时候，一旦遇到await就会先返回，等到异步操作完成，再接着执行函数体内后面的语句。函数前面的async关键字，表明该函数内部有异步操作。调用该函数时，会立即返回一个Promise对象。由于async函数返回的是Promise对象，可以作为await命令的参数。
>
**ES6 async函数有多种使用形式：**
>
> //函数声明
>
> async function foo(){}
>
> //函数表达式
>
> const foo = async function(){}
>
> 
>
> //对象的方法
>
> let obj = {async foo()}
>
> obj.foo().then(...)
>
> 
>
> //class方法
>
> class Storage{
>
> constructor(){
>
> this.cachePromise = cache.open("avatars")
>
> }
>
> async getAvatar(name){
>
> const cache = await this.cachePromise;
>
> return cache.match(`/avatars/${name}.jpg`)
>
> }
>
> }
>
>
**async与generator的区别?**
>
> async函数是Generator函数的语法糖，async函数就是将Generator函数的星号（*）替换成async，将yield替换成await。
>
> async函数对Generator函数的改进，体现在以下四点：
>
> 1、内置执行器
>
> 2、更好的语义：async表示函数里有异步操作，await表示紧跟在后面的表达式需要等待结果
>
> 3、更广的适用性：async函数的awai他命令后面，可以是Promise对象和原始类型的值（数字、字符串和布尔值，但这时等同于同步操作）
>
> 4、返回值是Promise：async函数的返回值是Peomise对象，这比Generator函数的返回值是Iterator对象方便对了，可以用then方法指定下一步的操作。
>
> 进一步说，async函数完全可以看作多个异步操作包装成的一个Promise对象，而await命令就是内部then命令的语法糖
>
> **简单实现****async/await中的async函数**
>
> async函数的实现原理，就是将Generator函数和自动执行器，包装在一个函数里
>
> function spawn(**genF**){
>
> **return** **new** Promise(function(**resolve**,**reject**){
>
> const gen **=** genF();
>
> function step(**nextF**){
>
> let next;
>
> *//ry/catch/finally 语句用于处理代码中可能出现的错误信息。*
>
> **try** {
>
> next **=** nextF()
>
> }**catch**(e){
>
> **return** reject(e);
>
> }
>
> **if**(next **.***done*){
>
> **return** resolve(next**.***value*);
>
> }
>
> Promise**.**resolve(next**.***value*)**.**then(
>
> function(**v**){
>
> step(function(){
>
> **return** gen**.**next(v)
>
> });
>
> },
>
> function(**v**){
>
> step(function(){
>
> **return** gen**.**throw(e)
>
> });
>
> }
>
> )
>
> }
>
> step(function(){
>
> **return** gen**.**next(undefined);
>
> });
>
> })
>
> }
>
> 
>
**有用过****promise吗？请写出下列代码的执行结果，并写出你的理解思路：**TODO
>
```
setTimeout(()=>{
​    console.log(1);
}, 0)
 new Promise((resolve)=>{
​    console.log(2);
​    for(var i = 1; i < 200; i++){
​        i = 198 && resolve()
​    }
​    console.log(3)
}).then(()=>{
​    console.log(4)
})
console.log(5)// 2 3 5 4 1 
```
> · 首先要讲一下，js是单线程执行，那么代码的执行就有先后; 
>
> · 有先后，那就要有规则(排队)，不然就乱套了，那么如何分先后呢？大体分两种：同步、异步; 
>
> · 同步很好理解，就不用多说了(我就是老大,你们都要给我让路); 
>
> · 异步(定时器[setTimeout ，setInterval]、事件、ajax、promise等)，说到异步又要细分宏任务、微任务两种机制， 
>
> · 宏任务：js异步执行过程中遇到宏任务，就先执行宏任务，将宏任务加入执行的队列(event queue),然后再去执行微任务; 
>
> · 微任务：js异步执行过程中遇到微任务，也会将任务加入执行的队列([event queue](https://www.toutiao.com/i6606779850801807885/))，但是注意这两个queue身份是不一样的，不是你先进来，就你先出去的（就像宫里的皇上选妃侍寝一样，不是你先进宫(或先来排队)就先宠幸的 ），真执行的时候是先微任务里拿对应回调函数，然后才轮到宏任务的队列回调执行的; 
>
> · 理解了这个顺序，那上面的结果也就不难懂了。
>
**Object.is（）与原来的比较操作符===，==的区别？**
>
> · ==相等运算符，比较时会自动进行数据类型转换
>
> · ===严格相等运算符，比较时不进行隐式类型转换
>
> · Object.is同值相等算法，在===基础上对0和NaN特别处理
>
> +0 === -0 //true
>
> NaN === NaN // false
>
> Object.is(+0, -0) // false
>
> Object.is(NaN, NaN) // true
>
> 
>
> **ES6新特性详细介绍说明：**
>
> **变量声明：****const和let：**
>
> ES6推荐使用let声明局部变量，相比之前的var（无论声明在何处，都会被视为声明在函数的最顶部），而let不会将声明变量提前；
>
> let表示声明变量，而const表示声明常量，两者都为块级作用域；const声明的变量都会被认为是常量，意思就是它的值被设置完成后就不能再修改了。
>
**注意：**let关键词声明的变量不具备变量提升的特性
>
> const和let声明只在最高进的一个块中（花括号内）有效
>
> const在声明时必须被赋值
>
>
**类和继承：**
>
> class和extend是一种语法糖，也是基于原型继承实现的
>
> class和super calls，实例化，静态方法和构造函数
>
> <script>
>
> ​    //class声明类 内部直接是属性和方法 不用,分隔。 constructor
>
> ​    class Person{
>
> ​      constructor(name, age){
>
> ​        this.name = name;//实例属性
>
> ​        this.age = age;
>
> ​        console.log(name,age)
>
> ​      }
>
> ​      sayhi(name){
>
> ​        //使用ES6新特性字符串模块,注意外层包裹符号是``反引号来创建字符串,内部变量使用${}
>
> ​        console.log(`this name is ${this.name}`);
>
> ​        //以往的写法
>
> ​        console.log('my age is '+this.age)
>
> ​      }
>
> ​    }
>
> ​    
>
> 
>
> ​    class Programmer extends Person{
>
> ​      constructor(name,age){
>
> ​        //直接调用父类结构器进行初始化
>
> ​        super(name,age)
>
> ​      }
>
> ​      program(){
>
> ​        console.log("I'm coding...")
>
> ​      }
>
> ​    }
>
> ​    var anim = new Person("张三",18);
>
> ​    anim.sayhi();
>
> ​    var wayou = new Programmer("李四",20);
>
> ​    wayou.sayhi();
>
> ​    wayou.program();
>
> ​    </script>
>
**字符串模板：**
>
> ES6中允许使用反引号` 来创建字符串，此方法创建的字符串里面可以包含由${ }包裹的变量
>
> <script>
>
> //产生一个随机数
>
> var num = Math.random();
>
> //将这个数字输出到console
>
> console.log(`输出随机数${num}`);
>
> </script>
>

>
> **解构：**
>
> 自动解析数组或对象中的值。若一个函数要函数要返回多个值，常规的做法是返回一个对象，将每个值作为这个对象的属性返回。在ES6中，利用解构这一特性，可以直接返回一个数组，然后数组中的值会自动被解析到对应接收该值得变量中。
>
> <script>
>
> var [x,y] = getVal(), //函数返回值解析
>
> ​    [name, ,age] = ["wayou","male","secrect"]; //数组解析
>
> function getVal(){
>
> ​    return [1,2];
>
> }
>
> console.log(`x:${x},y:${y}`); //x:1,y:2
>
> console.log(`name:${name},age:${age}`); //name:wayou,age:secrect
>
> </script>
>
> **参数默认值，不定参数，拓展参数：**
>
> **默认参数值：**
>
> 可以在定义函数的时候指定参数的默认值，而不用像以前那样通过逻辑或操作符来达到目的了。
>
> <script>
>
> //传统方式设置默认方式
>
> function sayHello(name){
>
> ​    var name = name||'dude';
>
> ​    console.log("Hello "+name);
>
> }
>
> sayHello(); //Hello dude
>
> sayHello("wayou"); //Hello wayou
>
> 
>
> 
>
> //ES6的默认参数
>
> function sayHello2(name = "dude"){
>
> ​    console.log("Hello "+name)
>
> }
>
> sayHello2(); //Hello dude
>
> sayHello2("wayou"); //Hello wayou
>
> </script>
>
> **不定参数（拓展符）：**
>
> 不定参数是在函数中使用命名参数同时接收不定数量的未命名参数。这只是一种语法糖，在以前的JavaScript代码中我们可以通过arguments变量来达到这一目的。不定参数的格式是三个句点后跟代表所有不定参数的变量名。比如下面这个例子中，...x代表了所有传入add函数的参数。
>
> <script>
>
> //将所有参数想加的函数
>
> function add(...x){
>
> ​    return x.reduce((m,n)=>m+n);
>
> }
>
> //传递任意个数的参数
>
> console.log(add(1,2,3)); //输出:6
>
> console.log(add(1,2,3,4,5)); //输出:15
>
> </script>
>
> reduce（）方法接收一个函数作为累加器，数组中的每个值（从左到右）开始缩减，最终计算为一个值。
>
> reduce（）可以作为一个高阶函数，用于函数的compose
>
> 注意：reduce（）对于空数组是不会执行回调函数的
>
> 拓展符：将一个数组转为用逗号分隔的参数序列。（若数组为空不产生任何效果）
>
> <script>
>
> var x = [1,2,3,4,5,6];
>
> console.log(x); //(6) [1, 2, 3, 4, 5, 6]
>
> console.log(...x); //1 2 3 4 5 6
>
> </script>
>
> **拓展参数：**
>
> 拓展参数则是另一种形式的语法糖，它允许传递数组或类数组直接作为函数的参数而不用通过apply。
>
> <script>
>
> var people = ['wayou','john','sherlock'];
>
> //sayHello函数来接收三个单独的参数
>
> function sayHello(people1,people2,people3){
>
> ​    console.log(`Hello ${people1},${people2},${people3}`)
>
> }
>
> //以前的方式,如果需要传递数组当参数,我们需要使用函数apply方法
>
> sayHello.apply(null,people); //Hello wayou,john,sherlock
>
> sayHello(...people); //Hello wayou,john,sherlock
>
> </script>
>
> **for of值遍历：**
>
> for in循环用于遍历数组，类数组或对象，ES6中新引入的for of循环功能相似，不同的是每次循环他提供的不是序号而是值
>
> <script>
>
> var someArray = ['a','b','c'];
>
> for(v of someArray){
>
> ​    console.log(v); //a,b,c
>
> }
>
> </script>
>
> **iterator/generator:**
>
> iterator：它是这么一个对象，拥有一个next方法，这个方法返回一个对象{done，value}，这个对象包含两个属性，一个布尔类型的done和包含任意值的value。
>
> iterable：这是这么一个对象，拥有一个obj[@@iterator]方法，这个方法返回一个iterator
>
> generator：它是一个特殊的iterator。反的next方法可以接收一个参数并且返回值取决于它的构造函数（generator function）。generator同时拥有一个throw方法。
>
> generator番薯：即generator的构造函数。此函数内可以使用yield关键字，在yield出现的地方可以通过generator的next或throw方法向外界传递值。generator函数是通过function*来声明的。
>
> yield关键字：它可以暂停函数的执行，随后可以再进入函数继续执行
>
> 具体详情：https://blog.domenic.me/es6-iterators-generators-and-iterables/
>
> **模块：**
>
> 在ES6标准中，Javascript原生支持module了。这种将JS代码分割成不同功能的小块进行模块化的概念是在一些三方规范中流行起来的，比如CommonJS和AMD模式。
>
> 将不同功能的代码分别写在不同文件中，各模块只需导出公共接口部分，然后通过模块的导入方式可以在其他地方使用。
>
> <script>
>
> //单独的js文件,如:point.js
>
> module "point" {
>
> ​    export class Point {
>
> ​      constructor (x,y){
>
> ​        publice x = x;
>
> ​        publice y = y;
>
> ​      }
>
> ​    }
>
> }
>
> 
>
> //在需要引用模块的js文件内
>
> //声明引用的模块
>
> module point from './point.js';
>
> //这里可以看出,尽管声明了引用的模块,还是可以通过指定需要的部分进行导入
>
> import Point from "point"
>
> var origin = new Ponit(0,0);
>
> console.log(origin)
>
> </script>
>
**Map、Set和WeakMap、WeakSet** TODO
>
> 这些是新加的集合类型，提供了更加方便的获取属性值的方法，不用像以前一样用hasOwnProperty来检查某个属性是属于原型链上的还是当前对象的。同时，在进行属性值添加与获取时有专门的get、set方法。
>
> //Sets
>
> var s = new Set();
>
> s.add("hello").add("goodbye").add("hello");
>
> s.size === 2;
>
> s.has("hello")===true;
>
> //Maps
>
> var m = new Map();
>
> m.set("hello",42);
>
> m.set(s,34);
>
> m.get(s) === 34;
>
> 我们会把对象作为一个对象的键来存放属性值，普通集合类型比如简单对象会阻止垃圾回收器对这些作为属性键存在的对象回收，偶造成内存泄露的危险。而weakMap，weakSet则更加安全些，这些作为属性键的对象如果没有别的变量在引用它们，则会被回收释放掉，具体还看下面的例子。
>
> //weak Maps
>
> var wm = new WeakMap();
>
> wm.set(s,{eatra:42});
>
> wm.size === undefined;
>
> 
>
> //weak Sets
>
> var ws = new WeakSet();
>
> ws.add({data:42}); //因为添加到ws的这个临时对象没有其他变量引用它,所以ws不会保存它的值,也就是说这次添加其实没有意思
>
**Proxies**
>
> proxy可以监听对象身上发生了什么事情，并在这些事情发生后执行一些相应的操作。一下子让我们对一个对象有了很强的跟踪能力，同时咋数据绑定方面也很有用处。
>
> <script>
>
> //定义被侦听的目标对象
>
> var engineer = {name:"Join",salary:50};
>
> //定义处理程序
>
> var interceptor = {
>
> ​    set:function(receiver,property,value){
>
> ​      console.log(property,"is changed to",value);
>
> ​      receiver[property] = value;
>
> ​    }
>
> }
>
> //创建代理以进行侦听
>
> engineer = new Proxy(engineer,interceptor);
>
> //做一些改动来触发代理
>
> engineer.salary = 60; //控制台输出:salary is changed to 60
>
> </script>
>
> 上面代码，我们已经添加了注释，这里进一步解释。对于处理程序，是在被侦听的对象身上发生了相应事件之后，处理程序里面的方法会被调用，上面例子中我们设置了set的处理函数，表明。如果我们侦听对象的属性被更改，也就是被set了，那这个处理程序就会被调用，同时通过参数能够的值是哪个属性被更改，更改为什么值
>
>
**Math、Number、String、Object的新API**
>
> 对Math、Number、String还有Object等添加了许多新的API。
>
>

>
> 浏览器
>
> **前端需要注意哪些****SEO？（搜索引擎优化）：**
>
> \1. 合理的title、description、keywords：搜索对着三项的权重逐个减小，title值强调中你的那即可，重要关键词出现不要超过2次，而且要靠前，不同页面title要有所不同；description把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面description有所不同；keywords列举出重要关键词即可
>
> \2. 语义化的HTML代码，符合W3C规范：语义化代码让搜索引擎容易理解网页。
>
> \3. 重要内容HTML代码放在最前：搜索引擎抓取HTML顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取。
>
> \4. 重要内容不要用js输出：爬虫不会执行JS获取内容
>
> \5. 非装饰性图片必须加alt
>
> \6. 少用iframe：搜索引擎不会抓取iframe中的内容
>
> \7. 提高网站速度：网站速度是搜索引擎排序的一个重要指标
>
> **前后端分离的项目如何****seo？（偏难）**
>
> 先去 [www.baidu.com/robots.txt](https://link.juejin.im/?target=https://www.baidu.com/robots.txt) 找出常见的爬虫，然后在nginx上判断来访问页面用户的User-Agent是否是爬虫，如果是爬虫就用nginx方向代理到我们自己用nodejs+puppeteer实现的爬虫服务器上，然后用你的爬虫服务器怕自己的前后端分离的前端项目页面，增加扒页面的接受延时，保证异步渲染的接口数据返回，最后得到了页面的数据，返还给来访问的爬虫即可。
>
> **移动端常见的兼容性问题****:**
>
> 随着手机的普及,移动端的开发也成了一个重要方向，但是由于设备的不统一，会造成一些兼容性问题。
>
> \1. 设置文字行高为字体行高，解决文字上下边留白问题
>
> \2. 给动态元素添加事件，需要使用事件委托（绑定到document），解绑也需要用委托的方式。苹果机点击事件不能触发。需要用touch系列事件
>
> \3. Img标签src属性无值（php渲染过的），在苹果机上显示无图片，在安卓机上显示图片裂开。可添加alt属性及值
>
> \4. 同一个标签多次绑定同一个事件（页面复杂情况容易出现这种情况，尽量避免这种情况），可以减少bug的出现，利于维护页面
>
> \5. 在rem自适应页面使用精灵图。会容易出现图片缺角的问题（约1-2像素）。解决办法：使装精灵图的盒子变大，让图片居中显示
>
> \6. 给选中的盒子增加一个标识，可以使用伪元素，减少标签的使用
>
> \7. 有横向滚动条的内容被垂直触摸，在IOS机上无法滚动页面
>
> \8. 当祖父元素使用overflow属性时，父元素采用transform属性会影响子元素定位position:absolute；导致子元素超出隐藏，建议用其他属性替换transform属性。
>
> \9. click事件在IOS系统上有时会失效，给绑定click事件的元素加上cursor：pointer解决
>
> \10. placeholder垂直居中问题：在IOS和Android中显示不同。解决方法是：在保证input输入文本垂直居中的条件下，给placehoder设置padding-top
>
> **如何优化****SPA(单页面Web应用)****应用的首屏加载速度慢的问题？**
>
> 1) 将公用的JS库通过script标签外部引入，减少app。bundel的大小，让浏览器并行下载资源文件，提高下载速度
>
> 2) 在配置路由时，页面和组件使用懒加载的方式引入，进一步缩小App。bundel的体积，在调用某个组件时再加载对应的js文件
>
> 3) 加一个首屏loading图，提升用户体验
>
> **网页从输入网址到渲染完成经历了哪些过程？**
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
