ѧϰ�﷨ʱ�����ʼ���

һ�����ݼ���(����json)��
���ֺ�����ͬ�����첽��
����ṹ��˳����䡢������䡢ѭ����䣩
�������ݸ�ʽ�����֣��ַ��������飬������json�����󣩵�ʹ�÷�ʽ
����4����﷨�ǹ���js�������̵Ļ�����





ѧϰJS��Ҫʼ��˼���������⡣

һ�����ݼ���(����)��

��ζ���һ������
��η��ʶ�������ԣ�
���ֺ�����ͬ�����첽��

��ζ��庯�����������﷨���巽ʽ�ͱ��ʽ���巽ʽ������
��ε���ͬ��������ͬ��������ô���ؽ����
��ε����첽�������첽������ô���ؽ����
����ṹ��˳����䡢������䡢ѭ����䣩

˳������ִ�����̡�
��������ִ�����̡�ʲô���ݲ��ܳ�Ϊ����������䣿���Ǳ��ʽ��
ѭ������ִ�����̡�ѭ�������������ԣ�ʲô�ǳ�ʼ����䣿ʲô��ѭ���ж�������ʲô���ۼ�����Ϊʲô��Ҫ�������Բ��ܱ�֤ѭ����ȷִ�С�
�������ݸ�ʽ�����֣��ַ��������飬������json�����󣩵�ʹ�÷�ʽ��

�ַ�����ô�����ƴ���ַ�����
���ֺ��ַ��������������������ַ���������𣿺Ͷ����أ���������ʽ�أ�
������ô���α����Ԫ�أ����ݿ���ɾ��Ԫ���𣿿��������𣿿���������
ʲô���ı��ʽ���ܵõ�����ֵ��������1���ַ���1���бȽϻ�õ�true����false��
��ô���ʶ�������ԣ����Ը�ĳ������̬�����������
ѧϰJS�﷨����֪ʶʱҪ�ѱ�����Ϊ�����������ʼ�ո����鱾�ߣ����˼·�ͱ�ǣ���ˡ�������ѧϰ�����ʽʱ��������Ҫ��һ�������ʽ����ʲô��ֵ���������¼���ݵı������𣿱������������ģ�����ô������Щ�����ԣ�ֻ������������������ա�





ѧϰ����ץס�⼸����

ʲô�Ǻ�����

���ֶ��庯���ķ�ʽ

���ֶ��庯����ʽ�Ĳ���


�����﷨��ʽ���塣
�������ʽ���塣

��ƪ�ĵ�����������ǰ�˹���ʦ�����ʵ�һ�����⡣

function print(content) {
  console.log(content);
}

var print = function (content) {
  console.log(content);
}
�������ֶ��巽ʽ�ֱ��ʲô��������ʲô��

���������Խ���ĳ���ͳ�ƣ���Լ70%�������ߴ𲻳�����������������⡣˵��ʲô��˵�������������νǰ�˹���ʦ����̫���ˡ�

�������������ֶ��巽ʽ������

�����﷨���巽ʽ
// ���Ǻ����﷨���巽ʽ
function print(content) {
  console.log(content);
}
�������ʽ���巽ʽ
// ���Ǳ��ʽ���巽ʽ
var print = function (content) {
  console.log(content);
}
��С�������ֶ��巽ʽ�����ǵĲ�����������ɡ�

�����﷨���巽ʽ

�ú����﷨����һ���������ܻ�ö�����ǰ���Ŵ���

����

// ���Ǻ����﷨���巽ʽ
function print(content) {
  console.log(content);
}

print('Hello, JS');

��ע���ȶ����ʹ�ã��������ܷ��Ϲ�ء�
��

print('Hello, JS');

// ���Ǻ����﷨���巽ʽ
function print(content) {
  console.log(content);
}

��ע������ȥ������ʹ���˲Ŷ��壬��������ô���ԣ�
��ʵ����������ʽ�ǵȼ۵ģ�ԭ����Ǵ�����ִ��֮ǰ�����������ͨ�������﷨����ĺ�����ǰ���塣�Ӷ���֤���������⴦���ú�����

���ʽ���巽ʽ

���ʽ���巽ʽ����ͨ���������һ������һ����⣩

����һ������������

var name = 'xiaoming';
�ַ���xiaoming��һ���ַ������ʽ

�ٱ���

var name = 'xu' + 'xiaoming'��
'xu' + 'xiaoming'��һ�����ʽ�������ʾ��������xuxiaoming�󣬰ѽ����ֵ���˱���name��

���Ϻܺ����ɡ�

�Ǻ������ʽ��

var print = function (content) {
  console.log(content);
}
��������ȫ�������ƣ�function(content) { console.log(content )} ����һ�����ʽ����������ʽ���Ƹ��˱���print����ô���ǾͿ��ԳƱ���print��һ�����������ˡ�

���������������print�����ǾͿ���ͨ��print����ִ�иú����ˡ�

var print = function (content) {
  console.log(content);
}

print('Hello��JS');
��Ȼprint��һ������������һ������û�ж���֮ǰ�϶��ǲ���ʹ�õ�����

print('Hello��JS'); // �ม���û������ô��ʹ�ã�

var print = function (content) {
  console.log(content);
}
����Ĵ���϶�����

���˾��ʣ������﷨���巨����ǰ��Ϊɶ�������ʽ���巨�Ͳ���ǰ�أ�

����������⣬����������ʽ���巨����ǰ���Ƕ�������ǲ�����ζ�Ŷ���ǰ���ء��Ǿ������ˡ�

������ʽ���巨

ֱ��ʹ�ñ��ʽ

�����﷨���巨����ǰ�Ŵ�����Ҳ����˵���ʽ���巨��û�м�ֵ����ֵ�ɴ��ˡ�

// ���Ǻ����﷨���巽ʽ
function print() {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
// ���Ǻ������ʽ���巽ʽ
var print = function () {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
էһ��������ûɶ���𰡡����Ƕ�����һ��������Ȼ�����setTimeout��5���Ӻ�ص�print��

��һ���Ľ���д�����ٿ���

setTimeout(function() {
  console.log('Hello, JS');
}, 5000);
��ʵsetTimeoutֻҪһ��������������һ���ͺá��Ǽ�Ȼ�ں������ʽ���巽ʽ�У��ǰ�һ���������ʽ��ֵ��һ��������������Ϊʲô����ֱ�ӰѺ������ʽ��setTimeout�أ���ȫ���ԡ�

�����ͱ��������һ�����������ˣ��ֽ�ʡʱ�䣬�����ֽ��պ���⡣

����˵����������ǲ���һ��һ���ġ�

����������
var name = 'xiaoming';
console.log(name);
����ʡһ������

console.log('xiaoming');
����������
var print = function() {
  console.log('Hello, JS');
}

setTimeout(print, 5000);
����ʡһ������

setTimeout(function() {
  console.log('Hello, JS');
}, 5000);
�ں����ж��庯��

function printWelcome(name) {
  var addWelcome = function() {
    return '��ã�' + name;
  }

  console.log(addWelcome());
}

printWelcome('xiaoming');
�Ҿ����㣬�������׺����᲻��~�β��ι���








����ʹ�ú����ķ�ʽ

ͬ��������
�첽������
���ֺ������ؽ���ķ�ʽ

�������ؽ����
callback���ؽ����
�������ؽ����ע���

ͬ���������Բ���callback���ؽ��������Ҫ��ô����
�첽����ֻ�ܲ���callback�������ս�����������첽��������Ҳ��һ����������ֵ���������ؽ��Ҫ���֡�



�������ؽ��

���綨��һ����ͺ���sum������һ����Ͷ�����

// ������ͺ���sum
function sum(a, b) {
  var c = a + b;
  return c;
}

// ����sum����������������ֵ��sum�Ĳ�������sum����ִ���겢�������ֵ������value
var value = sum(1, 2);
// ��ӡvalue��ֵ
console.log(value);
Ϊ�˸��õĿ�����������̣������ڴ����м����ӡ����ִ�����кš�

console.log('flow: 1');
// ������ͺ���sum
function sum(a, b) {
  console.log('flow: 2');
  var c = a + b;
  console.log('flow: 3');
  return c;
  console.log('flow: 4');
}

console.log('flow: 5');
// ����sum����������������ֵ��sum�Ĳ�������sum����ִ���겢�������ֵ������value
var result = sum(1, 2);
console.log('flow: 6');
// ��ӡresult��ֵ
console.log(result);
console.log('flow: 7');
����ִ�е�������

flow: 1
flow: 5
flow: 2
flow: 3
flow: 6
3
flow: 7
�ں���sum�ڣ�flow: 4�����ܱ�ִ�У���Ϊǰ��һ��return c�ᵼ��������������ִ�С�

callback���ؽ��

���綨��һ����ͺ���sum������һ����Ͷ�����

// ������ͺ���sum
function sum(a, b, callback) {
  var c = a + b;
  callback(c);
}

// ����һ��callback���������ڽ���sum�������ص�ֵ
function resultCallback(value) {
  console.log(value);
}

// ����sum����������������ֵ��sum�Ĳ�����ͬʱ��resultCallback����ȥ
var result = sum(1, 2, resultCallback);
// ��ӡvalue��ֵ
console.log(result);
��ӡ����ִ�����к�

console.log('flow: 1');
// ������ͺ���sum
function sum(a, b, callback) {
  console.log('flow: 2');
  var c = a + b;
  callback(c);
  console.log('flow: 3');
}

console.log('flow: 4');
// ����һ��callback���������ڽ���sum�������ص�ֵ
function resultCallback(value) {
  console.log('flow: 5');
  console.log(value);
  console.log('flow: 6');
}

console.log('flow: 7');
// ����sum����������������ֵ��sum�Ĳ�����ͬʱ��resultCallback����ȥ
var result = sum(1, 2, resultCallback);
console.log('flow: 8');
// ��ӡresult��ֵ
console.log(result);
console.log('flow: 9');
����ִ�е�������

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
�ں���sum�ڣ�û����ȷreturn���������ͨ��callback�������صĽ��������console.log(result)��result��һ��û�ж����ֵundefined��

��Ȼͬ����������ͨ���������غͼ�ӷ��صõ������Ĵ����������Ǽ�ӷ�����ͬ�������еĴ�����ڻ������㣬�������˴���ĸ��Ӷȡ�ͬ����������ļ�ӷ��ؽ��������һ�����¡�