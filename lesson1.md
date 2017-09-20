学习语法时的自问技巧

一个数据集合(对象、json)。
两种函数（同步、异步）
三大结构（顺序语句、条件语句、循环语句）
多种数据格式（数字，字符串，数组，布尔，json，对象）的使用方式
以上4大块语法是构建js代码流程的基础。





学习JS是要始终思考下面问题。

一个数据集合(对象)。

如何定义一个对象？
如何访问对象的属性？
两种函数（同步、异步）

如何定义函数？（函数语法定义方式和表达式定义方式的区别）
如何调用同步函数？同步函数怎么返回结果。
如何调用异步函数？异步函数怎么返回结果。
三大结构（顺序语句、条件语句、循环语句）

顺序语句的执行流程。
条件语句的执行流程。什么内容才能成为条件，是语句？还是表达式？
循环语句的执行流程。循环语句的三大特性：什么是初始化语句？什么是循环判断条件？什么是累加器？为什么需要三大特性才能保证循环正确执行。
多种数据格式（数字，字符串，数组，布尔，json，对象）的使用方式。

字符串怎么相加来拼接字符串？
数字和字符串可以相加吗？哪数组和字符串能相加吗？和对象呢？和其他格式呢？
数组怎么用游标访问元素？数据可以删掉元素吗？可以增加吗？可以排序吗？
什么样的表达式才能得到布尔值？将数字1和字符串1进行比较会得到true还是false？
怎么访问对象的属性？可以给某个对象动态的添加属性吗？
学习JS语法基础知识时要把被动变为主动。如果你始终跟着书本走，你的思路就被牵制了。比如在学习数组格式时，你首先要想一个数组格式存在什么价值？会带来记录数据的便利性吗？便利性体现在哪？该怎么利用这些便利性？只有这样你才能真正掌握。





学习函数抓住这几个点

什么是函数？

两种定义函数的方式

两种定义函数方式的差异


函数语法方式定义。
函数表达式定义。

这篇文档是我在面试前端工程师经常问的一个问题。

function print(content) {
  console.log(content);
}

var print = function (content) {
  console.log(content);
}
以上两种定义方式分别叫什么？差异是什么？

依据我面试结果的初步统计，大约70%的面试者答不出来，结果很让我意外。说明什么？说明绝大多数的所谓前端工程师基础太差了。

从术语上这两种定义方式有区别。

函数语法定义方式
// 这是函数语法定义方式
function print(content) {
  console.log(content);
}
函数表达式定义方式
// 这是表达式定义方式
var print = function (content) {
  console.log(content);
}
别小看这两种定义方式，它们的差异会把你给搞蒙。

函数语法定义方式

用函数语法定义一个函数，能获得定义提前的优待。

比如

// 这是函数语法定义方式
function print(content) {
  console.log(content);
}

print('Hello, JS');

备注：先定义后使用，呃。。很符合规矩。
和

print('Hello, JS');

// 这是函数语法定义方式
function print(content) {
  console.log(content);
}

备注：看上去好像先使用了才定义，呃。。怎么可以？
其实上面两种形式是等价的，原因就是代码在执行之前，编译器会把通过函数语法定义的函数提前定义。从而保证可以在任意处调用函数。

表达式定义方式

表达式定义方式和普通定义变量是一个道理（一样理解）

定义一个变量这样做

var name = 'xiaoming';
字符串xiaoming是一个字符串表达式

再比如

var name = 'xu' + 'xiaoming'；
'xu' + 'xiaoming'是一个表达式，这个表示计算出结果xuxiaoming后，把结果赋值给了变量name。

以上很好理解吧。

那函数表达式呢

var print = function (content) {
  console.log(content);
}
你现在完全可以类推，function(content) { console.log(content )} 就是一个表达式。把这个表达式复制给了变量print。那么我们就可以称变量print是一个函数变量了。

有了这个函数变量print，我们就可以通过print变量执行该函数了。

var print = function (content) {
  console.log(content);
}

print('Hello，JS');
既然print是一个函数变量，一个变量没有定义之前肯定是不能使用的啦。

print('Hello，JS'); // 喔喔。。没定义怎么能使用？

var print = function (content) {
  console.log(content);
}
上面的代码肯定出错。

有人就问，函数语法定义法能提前，为啥函数表达式定义法就不提前呢？

那我提个问题，如果函数表达式定义法能提前，那定义变量是不是意味着都提前了呢。那就乱套了。

深入表达式定义法

直接使用表达式

函数语法定义法有提前优待，那也不能说表达式定义法就没有价值。价值可大了。

// 这是函数语法定义方式
function print() {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
// 这是函数表达式定义方式
var print = function () {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
乍一看，上面没啥区别啊。都是定义了一个函数，然后调用setTimeout，5秒钟后回调print。

来一个改进的写法，再看看

setTimeout(function() {
  console.log('Hello, JS');
}, 5000);
其实setTimeout只要一个函数变量，给一个就好。那既然在函数表达式定义方式中，是把一个函数表达式赋值给一个函数变量，那为什么不能直接把函数表达式给setTimeout呢？完全可以。

这样就避免多命名一个函数变量了，又节省时间，代码又紧凑好理解。

你们说，下面代码是不是一样一样的。

变量的做法
var name = 'xiaoming';
console.log(name);
可以省一个变量

console.log('xiaoming');
函数的做法
var print = function() {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
可以省一个变量

setTimeout(function() {
  console.log('Hello, JS');
}, 5000);
在函数中定义函数

function printWelcome(name) {
  var addWelcome = function() {
    return '你好！' + name;
  }

  console.log(addWelcome());
}

printWelcome('xiaoming');
我就问你，函数里套函数酷不酷~晕不晕哈哈








两种使用函数的方式

同步函数。
异步函数。
两种函数返回结果的方式

立即返回结果。
callback返回结果。
两个返回结果的注意点

同步函数可以采用callback返回结果，但不要这么做。
异步函数只能采用callback返回最终结果。但调用异步函数本身也有一个立即返回值。两个返回结果要区分。



立即返回结果

比如定义一个求和函数sum并调用一次求和动作。

// 定义求和函数sum
function sum(a, b) {
  var c = a + b;
  return c;
}

// 调用sum函数，并传递两个值给sum的参数，当sum函数执行完并将结果赋值给变量value
var value = sum(1, 2);
// 打印value的值
console.log(value);
为了更好的看清楚整个流程，可以在代码中加入打印代码执行序列号。

console.log('flow: 1');
// 定义求和函数sum
function sum(a, b) {
  console.log('flow: 2');
  var c = a + b;
  console.log('flow: 3');
  return c;
  console.log('flow: 4');
}

console.log('flow: 5');
// 调用sum函数，并传递两个值给sum的参数，当sum函数执行完并将结果赋值给变量value
var result = sum(1, 2);
console.log('flow: 6');
// 打印result的值
console.log(result);
console.log('flow: 7');
代码执行的序列是

flow: 1
flow: 5
flow: 2
flow: 3
flow: 6
3
flow: 7
在函数sum内，flow: 4并不能被执行，因为前面一行return c会导致整个函数结束执行。

callback返回结果

比如定义一个求和函数sum并调用一次求和动作。

// 定义求和函数sum
function sum(a, b, callback) {
  var c = a + b;
  callback(c);
}

// 定义一个callback函数，用于接收sum函数返回的值
function resultCallback(value) {
  console.log(value);
}

// 调用sum函数，并传递两个值给sum的参数，同时把resultCallback传过去
var result = sum(1, 2, resultCallback);
// 打印value的值
console.log(result);
打印代码执行序列号

console.log('flow: 1');
// 定义求和函数sum
function sum(a, b, callback) {
  console.log('flow: 2');
  var c = a + b;
  callback(c);
  console.log('flow: 3');
}

console.log('flow: 4');
// 定义一个callback函数，用于接收sum函数返回的值
function resultCallback(value) {
  console.log('flow: 5');
  console.log(value);
  console.log('flow: 6');
}

console.log('flow: 7');
// 调用sum函数，并传递两个值给sum的参数，同时把resultCallback传过去
var result = sum(1, 2, resultCallback);
console.log('flow: 8');
// 打印result的值
console.log(result);
console.log('flow: 9');
代码执行的序列是

flow: 1
flow: 4
flow: 7
flow: 2
flow: 5
3
flow: 6
flow: 3
flow: 8
undefined
flow: 9
在函数sum内，没有明确return结果，而是通过callback函数返回的结果。所以console.log(result)的result是一个没有定义的值undefined。

虽然同步函数可以通过立即返回和间接返回得到函数的处理结果，但是间接返回在同步函数中的处理过于画蛇添足，还增加了代码的复杂度。同步函数处理的间接返回结果并不是一件好事。