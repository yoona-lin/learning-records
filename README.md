# learning-records

- 目录
  - [Firebug 与 Firefox](#Firebug与Firefox)
  - [webpack 与 vue 项目搭建流程](#webpack与vue项目搭建流程)
  - [浏览器开发者工具使用技巧](#浏览器开发者工具使用技巧)
  - [vuex 了解了解](#vuex了解了解)
  - [ECMAScript 6 入门](#ECMAScript6入门)
  - [github的Action学习](#github的Action学习)
  - [Ajax全接触](#Ajax全接触)
  - []()
  - []()

## Firebug与Firefox

> 看了一些关于firebug编辑器的操作，安装时才知道已经没更新了，取消了整个编辑器了，把它内置在Firefox浏览器的“开发者工具”一项中了，试着用了一下，是个很不错的前端编辑环境，感觉很不错，一些请求跟响应很清晰，对源码的编辑与修改也很方便，推荐

```shall
2019.10.29
```

## webpack与vue项目搭建流程

> 慕课网址：https://www.imooc.com/learn/935

> 课程讲了如何配置开发前端项目工程；实现一个简单的TODO应用：优化配置达到上线标准；

> 关于webpack项目的搭建流程，基本的流程，清晰易懂，多看，跟着搭建一遍

> 一个不错的分享：https://github.com/carrieguo/vue.js-todolist

> 整理出两个文件夹，分别是项目的静态搭建和完成打包配置，成功运行

```shall
2019.11.03
```

## 浏览器开发者工具使用技巧
> https://www.imooc.com/learn/759

> 很实用与详细的一个教程，很多没这么知道但好用的技巧，值得多看多用，特别是对js编程的调试

```shall
2019.11.05
```

## vuex了解了解

> https://vuex.vuejs.org/zh/

> Vuex 是一个专为 Vue.js 应用程序开发的状态管理模式。它采用集中式存储管理应用的所有组件的状态，并以相应的规则保证状态以一种可预测的方式发生变化。

> 把组件的共享状态抽取出来，以一个全局单例模式管理呢,在这种模式下，我们的组件树构成了一个巨大的“视图”，不管在树的哪个位置，任何组件都能获取状态或者触发行为！这是vuex的基本思想。

> 如果您的应用够简单，您最好不要使用 Vuex。一个简单的 store 模式就足够您所需了。但是，如果您需要构建一个中大型单页应用，您很可能会考虑如何更好地在组件外部管理状态，Vuex 将会成为自然而然的选择。

```shall
2019.11.12
```

## ECMAScript6入门

> 阮一峰老师的教材：https://es6.ruanyifeng.com/

let 与 const 命令
> let 声明变量的有效域情况，let声明的变量只在它所在的代码块有效，不存在变量提升

> const 声明只读常量，声明后立即初始化，不能更改

> 块级作用域 {} 的使用


变量的结构赋值
> 数组的对应赋值，一一对应

> 对象的结构赋值，变量必须与属性同名，才能取到正确的赋值

> 字符串也可以解构赋值,字符串被转换成了一个类似数组的对象

箭头函数
> var f = v => v;   // 等同于  var f = function (v) {  return v;  };

> var f = () => 5;  // 等同于  var f = function () { return 5 };

Symbol

> ES6 引入了一种新的原始数据类型Symbol，表示独一无二的值。它是 JavaScript 语言的第七种数据类型，前六种是：undefined、null、布尔值（Boolean）、字符串（String）、数值（Number）、对象（Object）。

> Symbol 值通过Symbol函数生成。let s = Symbol(); 这就是说，对象的属性名现在可以有两种类型，一种是原来就有的字符串，另一种就是新增的 Symbol 类型。

Set 和 Map 数据结构
> ES6 提供了新的数据结构 Set。它类似于数组，但是成员的值都是唯一的，没有重复的值。Set本身是一个构造函数，用来生成 Set 数据结构。const s = new Set();

> ES6 提供了 Map 数据结构。它类似于对象，也是键值对的集合，但是“键”的范围不限于字符串，各种类型的值（包括对象）都可以当作键。也就是说，Object 结构提供了“字符串—值”的对应，Map 结构提供了“值—值”的对应，是一种更完善的 Hash 结构实现。如果你需要“键值对”的数据结构，Map 比 Object 更合适。

Proxy
> Proxy 用于修改某些操作的默认行为，等同于在语言层面做出修改，所以属于一种“元编程”（meta programming），即对编程语言进行编程,
Proxy 可以理解成，在目标对象之前架设一层“拦截”，外界对该对象的访问，都必须先通过这层拦截，因此提供了一种机制，可以对外界的访问进行过滤和改写。Proxy 这个词的原意是代理，用在这里表示由它来“代理”某些操作，可以译为“代理器”。

> ES6 原生提供 Proxy 构造函数，用来生成 Proxy 实例。
var proxy = new Proxy(target, handler);

Promise 对象

> 所谓Promise，简单说就是一个容器，里面保存着某个未来才会结束的事件（通常是一个异步操作）的结果，等主线程运行结束再返回结果。从语法上说，Promise 是一个对象，从它可以获取异步操作的消息。Promise 提供统一的 API，各种异步操作都可以用同样的方法进行处理。

> Promise对象有以下两个特点。
（1）对象的状态不受外界影响。Promise对象代表一个异步操作，有三种状态：pending（进行中）、fulfilled（已成功）和rejected（已失败）。只有异步操作的结果，可以决定当前是哪一种状态，任何其他操作都无法改变这个状态。
（2）一旦状态改变，就不会再变，任何时候都可以得到这个结果。

Iterator 和 for...of 循环

> - 遍历器（Iterator）就是一种统一的接口机制，来处理所有不同的数据结构。它是一种接口，为各种不同的数据结构提供统一的访问机制。任何数据结构只要部署 Iterator 接口，就可以完成遍历操作（即依次处理该数据结构的所有成员）;
> - Iterator 的作用有三个：一是为各种数据结构，提供一个统一的、简便的访问接口；二是使得数据结构的成员能够按某种次序排列；三是 ES6 创造了一种新的遍历命令for...of循环，Iterator 接口主要供for...of消费。

> - 一个数据结构只要部署了Symbol.iterator属性，就被视为具有 iterator 接口，就可以用for...of循环遍历它的成员。也就是说，for...of循环内部调用的是数据结构的Symbol.iterator方法。
> -  for...of循环可以使用的范围包括数组、Set 和 Map 结构、某些类似数组的对象（比如arguments对象、DOM NodeList 对象）、后文的 Generator 对象，以及字符串。

> JavaScript 原有的for...in循环，只能获得对象的键名，不能直接获取键值。ES6 提供for...of循环，允许遍历获得键值。
```
var arr = ['a', 'b', 'c', 'd'];
for (let a in arr) {
  console.log(a); // 0 1 2 3
}
for (let a of arr) {
  console.log(a); // a b c d
}
```

Generator 函数

> - Generator 函数有多种理解角度。语法上，首先可以把它理解成，Generator 函数是一个状态机，封装了多个内部状态。执行 Generator 函数会返回一个遍历器对象，也就是说，Generator 函数除了状态机，还是一个遍历器对象生成函数。返回的遍历器对象，可以依次遍历 Generator 函数内部的每一个状态。
> - 形式上，Generator 函数是一个普通函数，但是有两个特征。一是，function关键字与函数名之间有一个星号；二是，函数体内部使用yield表达式，定义不同的内部状态（yield在英语里的意思就是“产出”）。

> - ES6 诞生以前，异步编程的方法，大概有下面四种。**回调函数、事件监听、发布/订阅、Promise 对象**；  Generator 函数将 JavaScript 异步编程带入了一个全新的阶段。
> - 异步:所谓"异步"，简单说就是一个任务不是连续完成的，可以理解成该任务被人为分成两段，先执行第一段，然后转而执行其他任务，等做好了准备，再回过头执行第二段。

async 函数

> ES2017 标准引入了 async 函数，使得异步操作变得更加方便。async 函数是什么？一句话，它就是 Generator 函数的语法糖。async函数就是将 Generator 函数的星号`（*）`替换成async，将yield替换成await。

> async函数返回一个 Promise 对象，可以使用then方法添加回调函数。当函数执行的时候，一旦遇到await就会先返回，等到异步操作完成，再接着执行函数体内后面的语句。

Class 的基本语法

> ES6 提供了更接近传统语言的写法，引入了 Class（类）这个概念，作为对象的模板。通过class关键字，可以定义类。基本上，ES6 的class可以看作只是一个语法糖，新的class写法只是让对象原型的写法更加清晰、更像面向对象编程的语法而已。

> constructor方法是类的默认方法，通过new命令生成对象实例时，自动调用该方法。一个类必须有constructor方法，如果没有显式定义，一个空的constructor方法会被默认添加。

> Class 可以通过extends关键字实现继承，这比 ES5 的通过修改原型链实现继承，要清晰和方便很多

Module 的语法

> ES6 在语言标准的层面上，实现了模块功能，而且实现得相当简单，完全可以取代 CommonJS 和 AMD 规范，成为浏览器和服务器通用的模块解决方案。ES6 模块不是对象，而是通过export命令显式指定输出的代码，再通过import命令输入。

> - 模块功能主要由两个命令构成：export和import。export命令用于规定模块的对外接口，import命令用于输入其他模块提供的功能。
> - 一个模块就是一个独立的文件。该文件内部的所有变量，外部无法获取。如果你希望外部能够读取模块内部的某个变量，就必须使用export关键字输出该变量.

> - export命令规定的是对外的接口，必须与模块内部的变量建立一一对应关系。
> - export语句输出的接口，与其对应的值是动态绑定关系，即通过该接口，可以取到模块内部实时的值。
> - export命令可以出现在模块的任何位置，只要处于模块顶层就可以。如果处于块级作用域内，就会报错，下一节的import命令也是如此。这是因为处于条件代码块之中，就没法做静态优化了

> - 使用export命令定义了模块的对外接口以后，其他 JS 文件就可以通过import命令加载这个模块。
> - 如果想为输入的变量重新取一个名字，import命令要使用as关键字，将输入的变量重命名。import { lastName as surname } from './profile.js';
> - 由于import是静态执行，所以不能使用表达式和变量，这些只有在运行时才能得到结果的语法结构

> - export default 命令
> - 为了给用户提供方便，让他们不用阅读文档就能加载模块，就要用到export default命令，为模块指定默认输出。
> - `xport default function () {console.log('foo');} `  代码是一个模块文件export-default.js，它的默认输出是一个匿名函数（不管模块内是否为非匿名函数）。其他模块加载该模块时，import命令可以为该匿名函数指定任意名字。 

Module 的加载实现

> 默认情况下，浏览器是同步加载 JavaScript 脚本，即渲染引擎遇到<script>标签就会停下来，等到执行完脚本，再继续向下渲染。如果是外部脚本，还必须加入脚本下载的时间。如果脚本体积很大，下载和执行的时间就会很长，因此造成浏览器堵塞，用户会感觉到浏览器“卡死”了，没有任何响应。
  
> - defer与async的区别是：defer要等到整个页面在内存中正常渲染结束（DOM 结构完全生成，以及其他脚本执行完成），才会执行；async一旦下载完，渲染引擎就会中断渲染，执行这个脚本以后，再继续渲染。一句话，defer是“渲染完再执行”，async是“下载完就执行”。
> - 浏览器对于带有type="module"的<script>，都是异步加载，不会造成堵塞浏览器，即等到整个页面渲染完，再执行模块脚本，等同于打开了<script>标签的defer属性。
> - <script>标签的async属性也可以打开，这时只要加载完成，渲染引擎就会中断渲染立即执行。执行完成后，再恢复渲染。

编程风格

> 块级作用域
> - （1）let 取代 var：ES6 提出了两个新的声明变量的命令：let和const。其中，let完全可以取代var，因为两者语义相同，而且let没有副作用。
> - （2）全局常量和线程安全：在let和const之间，建议优先使用const，尤其是在全局环境，不应该设置变量，只应设置常量。const优于let有几个原因。const提醒变量不改变；const比较符合函数式编程思想，运算不改变值，只是新建值，而且这样也有利于将来的分布式运算；是 JavaScript 编译器会对const进行优化，所以多使用const，有利于提高程序的运行效率。

> 字符串
> - 静态字符串一律使用单引号或反引号，不使用双引号。动态字符串使用反引号

> 解构赋值
> - 使用数组成员对变量赋值时，优先使用解构赋值。函数的参数如果是对象的成员，优先使用解构赋值

> 对象
> - 单行定义的对象，最后一个成员不以逗号结尾。多行定义的对象，最后一个成员以逗号结尾

> 数组
> - 使用扩展运算符（...）拷贝数组,`const itemsCopy = [...items];`

> 函数
> - 立即执行函数可以写成箭头函数的形式。
```
(() => {
  console.log('Welcome to the Internet.');
})();
```
> - 那些使用匿名函数当作参数的场合，尽量用箭头函数代替。因为这样更简洁，而且绑定了 this

> Map 结构
> - 注意区分 Object 和 Map，只有模拟现实世界的实体对象时，才使用 Object。如果只是需要key: value的数据结构，使用 Map 结构。因为 Map 有内建的遍历机制

> Class
> - 总是用 Class，取代需要 prototype 的操作。因为 Class 的写法更简洁，更易于理解
> - 使用extends实现继承，因为这样更简单，不会有破坏instanceof运算的危险

> 模块
> - 首先，Module 语法是 JavaScript 模块的标准写法，坚持使用这种写法。使用import取代require。
> - 使用export取代module.exports。
> - 如果模块默认输出一个函数，函数名的首字母应该小写。`function makeStyleGuide() {} export default makeStyleGuide;`
> - 如果模块默认输出一个对象，对象名的首字母应该大写。`const StyleGuide = {es6: {}};export default StyleGuide;`

> ESLint 的使用
> - ESLint 是一个语法规则和代码风格的检查工具，可以用来保证写出语法正确、风格统一的代码。

ArrayBuffer
> - ArrayBuffer对象、TypedArray视图和DataView视图是 JavaScript 操作二进制数据的一个接口。
> - ArrayBuffer对象代表原始的二进制数据，TypedArray视图用来读写简单类型的二进制数据，DataView视图用来读写复杂类型的二进制数据。
> - ArrayBuffer对象代表储存二进制数据的一段内存，它不能直接读写，只能通过视图（TypedArray视图和DataView视图)来读写，视图的作用是以指定格式解读二进制数据。ArrayBuffer也是一个构造函数，可以分配一段可以存放数据的连续内存区域。

```shall
2019.11.12 - 2019.11.15
```

## github的Action学习

> 阮一峰老师的日记：http://www.ruanyifeng.com/blog/2019/09/getting-started-with-github-actions.html

> GitHub Actions 是什么？
> - 大家知道，持续集成由很多操作组成，比如抓取代码、运行测试、登录远程服务器，发布到第三方服务等等。GitHub 把这些操作就称为 actions。
> - 很多操作在不同项目里面是类似的，完全可以共享。GitHub 注意到了这一点，想出了一个很妙的点子，允许开发者把每个操作写成独立的脚本文件，存放到代码仓库，使得其他开发者可以引用。
> - 如果你需要某个 action，不必自己写复杂的脚本，直接引用他人写好的 action 即可，整个持续集成过程，就变成了一个 actions 的组合。这就是 GitHub Actions 最特别的地方。

> GitHub Actions 有一些自己的术语。
> - （1）workflow （工作流程）：持续集成一次运行的过程，就是一个 workflow。
> - （2）job （任务）：一个 workflow 由一个或多个 jobs 构成，含义是一次持续集成的运行，可以完成多个任务。
> - （3）step（步骤）：每个 job 由多个 step 构成，一步步完成。
> - （4）action （动作）：每个 step 可以依次执行一个或多个命令（action）。

> 看不懂啊

> 实例
> - 第一步，这个示例需要将构建成果发到 GitHub 仓库，因此需要 GitHub 密钥。按照官方文档，生成一个密钥。然后，将这个密钥储存到当前仓库的Settings/Secrets里面。
> - 第二步，本地计算机使用create-react-app，生成一个标准的 React 应用。然后，打开package.json文件，加一个homepage字段，表示该应用发布后的根目录
> - 第三步，在这个仓库的.github/workflows目录，生成一个 workflow 文件，名字可以随便取，这个示例是ci.yml。
> - 第四步，保存上面的文件后，将整个仓库推送到 GitHub。GitHub 发现了 workflow 文件以后，就会自动运行。你可以在网站上实时查看运行日志，日志默认保存30天。等到 workflow 运行结束，访问 GitHub Page，会看到构建成果已经发上网了。以后，每次修改后推送源码，GitHub Actions 都会自动运行，将构建产物发布到网页。

> 还是不懂，等看看有没有视频教程

```shall
2019.11.16
```

## Ajax全接触

> Ajax全接触: https://imooc.com/learn/250

AJAX
> - AJAX:Asynchronous and JavaScript and XML（异步的JavaScript 和 XML）
> - AJAX不是某种编程语言，是一种在无需加载整个网页的情况下局部更新部分网页的技术
> - 正常情况下更新与提交表单时都要重新加载整个页面

异步
> - XMLHTTPRequest实现前台与服务器之间的数据交互
> - 运用HTML与CSS来实现页面，表达展示信息
> - 运用XMLHTTPRequest和Web服务器来进行数据的异步交互
> - 运用JavaScript操作DOM，实现动态局部更新刷新

XMLHTTPRequest
> - 初始化对象：var request = new XMLHTTPTRequest();
> - 考虑兼容性
```javascript
    var request;
    if(window.XMLHttpRequest){
      request = new XMLHttpRequest();//IE+，Firefox，Chrome，Opera、、、
    }else{
      request = new ActionXObject("Microsoft.XMLHTTP");//IE6,IE5
    }
```

Http
> - http是计算机通过网络进行通信的规则
> - HTTP是一种无状态协议，不建立持久的连接

> - 一个完整的HTTP请求过程，通常有下面7个步骤
> - 1.建立TCP连接
> - 2.Web浏览器先Web服务器发送请求命令
> - 3.Web浏览器发送请求头信息
> - 4.Web服务器应答
> - 5.Web服务器发送应答头信息
> - 6.Web服务器向浏览器发送数据
> - 7.Web服务器关闭TCP连接

> - HTTP请求
> - 一个HTTP请求一般由四部分组成
> - 1.HTTP请求的方法或动作，比如是GET还是POST请求
> - 2.正在请求的URL
> - 3.请求头，包含一些客户端环境信息，身份验证信息等（请求头与请求体之间有个空行）
> - 4.请求体，也就是请求正文，请求正文包含客户提交的查询字符串信息，表单信息等等
```
    GET /Protocols/rfc2616/rfc2616-sec5.html HTTP/1.1
    Host: www.w3.org
    Connection: keep-alive
    Cache-Control: max-age=0
    Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8
    User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.153 Safari/537.36
    Referer: https://www.google.com.hk/
    Accept-Encoding: gzip,deflate,sdch
    Accept-Language: zh-CN,zh;q=0.8,en;q=0.6
    Cookie: authorstyle=yes
    If-None-Match: "2cc8-3e3073913b100"
    If-Modified-Since: Wed, 01 Sep 2004 13:24:52 GMT

    name=qiu&age=25
```
> - GET：一般用于信息获取，信息查询，所以对服务器信息安全；使用URL传递参数，但参数所有人可见；对所发信息数量也有限制，一般在2000个字符
> - POST：一般用于修改服务器上的资源，修改操作；对所发信息数量无限制

> - 一个HTTP相应一般由三部分组成
> - 1.一个数字和文字组成的状态码，用来显示请求是否成功还是失败
> - 2.响应头，响应头也和请求头一样包含许多有用的信息，例如服务器类型、日期时间、内容类型和长度等（与相应体之间也是有一行空行）
> - 相应体，也就是相应正文
```
    HTTP/1.1 200 OK
    Date: Tue, 08 Jul 2014 05:28:43 GMT
    Server: Apache/2
    Last-Modified: Wed, 01 Sep 2004 13:24:52 GMT
    ETag: "40d7-3e3073913b100"
    Accept-Ranges: bytes
    Content-Length: 16599
    Cache-Control: max-age=21600
    Expires: Tue, 08 Jul 2014 11:28:43 GMT
    P3P: policyref="http://www.w3.org/2001/05/P3P/p3p.xml"
    Content-Type: text/html; charset=iso-8859-1

    {"name": "qiu", "age": 25}
```

> - HTTP 状态码
> - 1XX：消息，这一类型的状态码，代表请求已被接受，需要继续处理
> - 2XX：成功，这一类型的状态码，代表请求已成功被服务器接收、理解、并接受，如 200 OK
> - 3XX：重定向，这类状态码代表需要客户端采取进一步的操作才能完成请求
> - 4XX：请求错误，这类的状态码代表了客户端看起来可能发生了错误，妨碍了服务器的处理，如 404 MOT
> - 5XX：服务器错误，这类状态码代表了服务器在处理请求的过程中有错误或者异常状态发生，也有可能是服务器意识到以当前的软硬件资源无法完成对请求的处理，如 500

XMLHTTPRequest 发送请求
```
open(method,url,async)   //用于调用HTTP请求（发送请求方法，请求地址，是否异步操作默认true）
send(string);  //发送请求到服务器

request.open("GET","get.php",true);
request.send();

request.open("POST","get.php",true);
request.send();  //这里是POST但是没给出参数，实际应用很少

request.open("POST","get.php",true);
request.setRequestHeader("Content-type","application/x-www-form-urlencoded");
request.send("name=王二狗&sex=男");
```

XMLHTTPRequest 接受相应
```
responseText: 获得字符串形式的响应数据
responseXML: 获得XML形式的响应数据（用的较少，大多数情况用JSON）
status, statusText: 以数字和文本形式返回HTTP状态码
getAllResponseHeader(): 获取所有的响应报头
getResponseHeader(参数): 查询响应中某个字段的值

readyState属性
readyState: 响应是否成功
0：请求为初始化，open还没有调用
1：服务器连接已建立，open已经调用了
2：请求已接收，接收到头信息了
3：请求处理中，接收到响应主题了
4：请求已完成，且响应已就绪，也就是响应完成了

监听readyState属性的变化：

var request = new XMLHttpRequest();
request.open("GET", "get.php", true);
request.send();
//该属性每次变化时会触发
request.onreadystatechange = function(){
    //若响应完成且请求成功
    if(request.readyState === 4 && request.status === 200){
        //do something, e.g. request.responseText
    }
}
```

PHP
> - 1.PHP 简介：是一种创建动态交互性站点的服务器端脚本语言。
> - 2.PHP的作用：能够生成动态页面内容；能够创建、打开、读取、写入、删除以及关闭服务器上的文件；能够接收表单数据；能够发送并取回cookies； 能够添加删除修改数据库中的数据；能够限制用户访问网站中的某些页面
> - 3.调试器下载：https://www.apachefriends.org/download.html

JSON
> - JSON：JavaScript 对象表示法（JavaScript Object Notation）
> - JSON 是存储和交换文本信息的语法，类似于 XML，它采用键值对的方式来组织，易于阅读和编写，同时也易于机器的解析与生成
> - JSON 是独立于语言的，也就是说不管什么语言，都可以解析json，只需要按照json的规则来解析就行

> - json的长度比XML短，读写速度更快
> - json可以使用JavaScript内置的方法直接进行解析，转换成JavaScript对象

> JSON数据由花括号括起来，可以包含多个“名称：值”对，以逗号隔开
```
    {
      "name":"lin",
      "age":23,
      "sex":"男",
      "school":{
        "sname":"广东工业大学",
        "address":"101"
      },
      "array":[
        {"one":"one","age":20},
        {"two":"two","age":22}
      ]
    }
```
> JSON数据的“名称：值”中的值可以是多种数据类型，如：1、数字（整数或浮点数）2、字符串（在双引号中）3、逻辑值（true 或 false）4、数组（在方括号中）5、对象（在花括号中）6、null

> 校验工具：https://jsonlint.com/

> - JSON解析
> - eval 和 JSON.parse
> - 在代码中使用eval是很危险的！！特别是用他执行第三方的JSON数据（其中可能包含恶意代码）时，尽可能使用JSON.parse()方法解析字符串本身，该方法还可以捕捉JSON数据中的语法错误

jQuery中的AJAX

> jQuery.ajax([settings])
```
type：类型，“POST”或“GET”，默认为GET
url：发送请求的地址
data：是一个对象，连同请求发送到服务器的数据
dataType：预设服务器返回的数据类型，如果不指定，jQuery将自动根据HTTP包MIME信息来智能判断，一般我们采用json格式，可以设置“json”
success：是一个方法，请求成功后的回调函数，传入返回后的数据，以及包含成功代码的字符串
error：是一个方法，请求失败是调用此函数，传入XMLHTTPRequest对象

$.ajax({
    //请求方式
    type:'POST',
    //发送请求的地址
    url:'fzz.php',
    //服务器返回的数据类型
    
    type:'GET',
    //发送请求的地址以及传输的数据
    url:'fzz.php?number'+=xxx,
    //服务器返回的数据类型
    
    //下面部分一样
    dataType:'json',
    //发送到服务器的数据，对象必须为key/value的格式，jquery会自动转换为字符串格式
    data:{name:xxx,age:xxx},
    success:function(data){
        //请求成功函数内容
    },
    error:function(jqXHR){
        //请求失败函数内容
    }
});
```

跨域
> - JavaScript出于安全方面的考虑，不允许跨域调用其他页面的对象，什么是跨域呢？就是因为JavaScript同源策略的限制,a.com 域名下的js无法操作 b.com 或是 c.b.com 域名下的对象
> - 域名组成： `http://`(协议) `wwww`(子域名) . `abc.com`(主域名) : `8080`(端口号) /  `script/jquery.js`(请求资源地址) 
> - 当协议、子域名。主域名、端口号任意一个不同时，都算作不同的域
> - 不同域之间的相互请求资源就算是“跨域”

处理跨域方式
> - 1.代理：通过在同域名的web服务器创建一个其他域的代理,这种方式是通过后台(ASP、PHP、JAVA、ASP.NET)获取其他域名下的内容，然后再把获得内容返回到前端，这样因为在同一个域名下，所以就不会出现跨域的问题。
> - 2.JSONP：JSONP 可用于解决主流浏览器的跨域数据访问的问题（注意：JSONP支持GET方式调用,不支持POST请求）
> - 3.XHR2: XMLHttpRequest Level 2,HTML5提供的XMLHttpRequest Level 2已经实现了跨域访问以及其他的一些新功能（只支持HTML5，如果你是移动端开发，可以选择使用XHR2）
```
XHR2需要在远程服务器端添加如下代码
header('Access-Control-Allow-Origin:*'); //*代表可访问的地址，可以设置指定域名
header('Access-Control-Allow-Methods:POST,GET');
```

> 课程源码在上面

```shall
2019.11.19
```
