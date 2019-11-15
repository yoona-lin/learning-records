# learning-records

- 目录
  - [Firebug 与 Firefox](#Firebug与Firefox)
  - [webpack 与 vue 项目搭建流程](#webpack与vue项目搭建流程)
  - [浏览器开发者工具使用技巧](#浏览器开发者工具使用技巧)
  - [vuex 了解了解](#vuex了解了解)
  - [ECMAScript 6 入门](#ECMAScript6入门)
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
