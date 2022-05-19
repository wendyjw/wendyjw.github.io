## 通用型

> 开放性题目


- 你最近遇到的技术挑战是什么？你是如何解决的？
- 在创建或维护一个网站时，你能否说下用来提高性能的一些技术？
- 了解 SEO 吗，请描述一下你最近使用的一些 SEO 最佳实践或技术。
- 你能解释一下前端安全方面的常见技术或最近解决的问题吗？
- 在最近的项目中，你个人采取了哪些措施来提高代码的可维护性？
- 你能描述渐进增强和优雅退化之间的区别吗？
- 描述一下你将如何创建一个简单的幻灯片页面。
- 如果你今年能掌握一项技术，那会是什么？
- 了解 CORS 吗？它解决了什么问题？
- 你是如何处理与上司或同事的分歧的？
- 你使用哪些资源来了解最新的前端技术。
- 你有什么自己的周末项目吗？
- 当初为什么选择做前端开发？
- React 的虚拟 DOM 比操作原生 DOM 快吗？虚拟 DOM 的初衷。
- 什么是 SPA 单页应用？
- git 用过吗，上家公司开发新功能到上线分支是如何管理的。

## HTML

- 描述 cookie、sessionStorage 和 localStorage 之间的区别。
- 描述`<script>`、`<script async>`和`<script defer>`之间的区别。
- 为什么我们页面通常要将 CSS`<link>`放在`<head></head>`中并放在`<script>`的前面？
- 什么是渐进式渲染？
- img 标签的 srcset 属性是干嘛的？说一下浏览器是如何处理该属性的。

## CSS

- 描述 BFC 及其工作原理。
- 在项目实践中，是如何处理不同浏览器样式兼容问题的？
- 有哪些是可以隐藏内容的属性，它们之间有什么区别？
- 伪元素和伪类的区别。
- inline 和 inline-block 的区别。
- 列举几种垂直居中的方法。
- 如何实现多行文本溢出省略。
- flex 布局的 flex 属性是什么的缩写。
- 逻辑像素和物理像素的区别，px 属于什么像素。

## JavaScript

- 什么是闭包，列举一个使用案例。
- `==`和`===`之间的区别是什么？
- 解释 mutable 和 immutable 之间的区别。
- 简单介绍下 event loop。
- 列举下 JS 的几种基本类型。
- typeof 和 instanceof。
- 什么是防抖和节流？有什么区别？如何实现？
- 多个 tab 只对应一个内容框，点击每个 tab 都会请求接口并渲染到内容框，怎么确保频繁点击 tab 但能够确保数据正常显示？

## Performance

- 你是如何对网页做性能分析的？
- 动画性能如何检测？
[https://github.com/lgwebdream/FE-Interview/issues/922](https://github.com/lgwebdream/FE-Interview/issues/922)
- 列表页跳转到详情页，详情页数据接口很慢，前端可以怎么优化用户体验？
[https://github.com/lgwebdream/FE-Interview/issues/929](https://github.com/lgwebdream/FE-Interview/issues/929)
- 页面有个自动滚动窗口，同时只显示 10 条数据，但数据源有 100 条，如何优化？
虚拟列表

## Network

- 输入 URL 到整个网页加载完毕的过程。
- 轮询和 websocket 的使用场景。
- 简单讲解一下 HTTP2 的多路复用。
- 浏览器出现 from disk、from memory 的策略是什么？
- 状态码 302、401、403。

## Webpack

- webpack 中 loader 和 plugin 的区别是什么？
- 热更新的原理。
- tree-shaking 原理，package.json 中的 sideEffects 什么作用。

## React

- React.Component 和 React.PureComponent 的区别。
- React 的 useEffect、useCallback、useMemo。
- hooks 为什么要保证严格的执行顺序，不能放在条件表达式中。

### 问题代码分析
| 下面代码执行会报Warning, 分析报错原因 : 
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648034735506-571a0d55-2ab1-45dc-8221-9086c073c31c.png#clientId=ua4ed67de-3f83-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=284&id=u32f7668b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=446&originWidth=890&originalType=binary&ratio=1&rotation=0&showTitle=false&size=128465&status=done&style=none&taskId=ub0e47b31-297d-40a0-8811-01de2cb05ec&title=&width=567)
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648034769547-46b94a6f-dc43-4764-abcc-888608c79c23.png#clientId=ua4ed67de-3f83-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=28&id=u5a32d408&margin=%5Bobject%20Object%5D&name=image.png&originHeight=28&originWidth=320&originalType=binary&ratio=1&rotation=0&showTitle=false&size=7297&status=done&style=none&taskId=uf50d7140-f70e-46a6-9a7f-965160b5324&title=&width=320) |
| --- |
| 下面代码在点击一次button后, 为什么counter会变成1, 而不是2, 这不符合我们的预期, 如何保证counter变成2?
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648036485921-c80d8c7c-0c5e-4bb3-ae33-3e999589a1f7.png#clientId=uaf0c9b3d-0355-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=406&id=u6d857168&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1096&originWidth=1346&originalType=binary&ratio=1&rotation=0&showTitle=false&size=334698&status=done&style=none&taskId=uf4a95d59-a0ed-42c6-a7da-c198d411580&title=&width=498) |
| 下面代码在点击button之后, 页面显示的点击次数依然是0, 为什么?
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648036764570-7e092699-a178-4dc4-9614-aa5a5dd99ecb.png#clientId=uaa390338-689e-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=378&id=ua55371cb&margin=%5Bobject%20Object%5D&name=image.png&originHeight=802&originWidth=898&originalType=binary&ratio=1&rotation=0&showTitle=false&size=190413&status=done&style=none&taskId=u5ff79c56-181a-42a3-b0f8-ca70a614827&title=&width=423) |
| 下面代码在点击button后会依次输出什么信息, 为什么?
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648037987291-6190e22b-7b4c-455d-bad6-874d7b0bf7ca.png#clientId=u17f62683-a994-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=463&id=ubb94b059&margin=%5Bobject%20Object%5D&name=image.png&originHeight=960&originWidth=1402&originalType=binary&ratio=1&rotation=0&showTitle=false&size=242289&status=done&style=none&taskId=u3a8f34d9-81fc-42bd-8eda-0c52031638b&title=&width=676) |
| 现有如下代码
index.js
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648090027739-65e99b1a-af15-4e8c-8901-af1a53b9eeda.png#clientId=u5c192d58-1387-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=190&id=u7ccf4e94&margin=%5Bobject%20Object%5D&name=image.png&originHeight=262&originWidth=718&originalType=binary&ratio=1&rotation=0&showTitle=false&size=66786&status=done&style=none&taskId=u4279de0d-0432-4ea3-906a-34f1ef74185&title=&width=520)
Test.jsx
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648090058584-eea215c1-a025-407e-8454-791804dc7e51.png#clientId=u5c192d58-1387-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=172&id=u30f326c3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=308&originWidth=934&originalType=binary&ratio=1&rotation=0&showTitle=false&size=87853&status=done&style=none&taskId=u4ff94710-cc64-4e00-a363-57a938ebf44&title=&width=523)
上面代码执行报错 
![image.png](https://cdn.nlark.com/yuque/0/2022/png/22762486/1648090152483-cb3c787f-c691-4793-af31-fea6f3789425.png#clientId=u5c192d58-1387-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=105&id=u2934336e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=105&originWidth=589&originalType=binary&ratio=1&rotation=0&showTitle=false&size=29447&status=done&style=none&taskId=u6a80d612-306b-4a73-9376-d8153e7583b&title=&width=589)
请分析报错原因, 以及如何解决该报错. |
|  |



## Coding

```javascript
// 输出结果
var foo = 10 + '20';

// 输出结果
'Good Luck'
  .split('')
  .reverse()
  .join('');

// foo.x最终等于什么
var foo = { n: 1 };
var bar = foo;
foo.x = foo = { n: 2 };

// 输出结果
async function async1() {
  console.log('1');
  await async2();
  console.log('2');
}
async function async2() {
  console.log('3');
}
console.log('4');
setTimeout(function() {
  console.log('5');
}, 0);
async1();
new Promise(function(resolve) {
  console.log('6');
  resolve();
}).then(function() {
  console.log('7');
});
console.log('8');

// 输出结果
const list = [1, 2, 3];
const square = num => {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve(num * num);
    }, 1000);
  });
};
function test() {
  list.forEach(async x => {
    const res = await square(x);
    console.log(res);
  });
}
test();

// 扁平化该数组
var arr = [[1, 2, 2], [3, 4, 5, 5], [6, 7, 8, 9, [11, 12, [12, 13, [14]]]], 10];

// 输出结果
class Example extends React.Component {
  constructor() {
    super();
    this.state = {
      val: 0,
    };
  }
  componentDidMount() {
    this.setState({ val: this.state.val + 1 });
    console.log(this.state.val); // 第 1 次 log
    this.setState({ val: this.state.val + 1 });
    console.log(this.state.val); // 第 2 次 log
    setTimeout(() => {
      this.setState({ val: this.state.val + 1 });
      console.log(this.state.val); // 第 3 次 log
      this.setState({ val: this.state.val + 1 });
      console.log(this.state.val); // 第 4 次 log
    }, 0);
  }
  render() {
    return null;
  }
}

// 输出结果，如何改造输出1-9
for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    console.log(i);
  }, 1000);
}

// 将数组按照age从小到大排列
var arr = [{ age: 24 }, { age: 15 }, { age: 20 }, { age: 14 }];

// 一个构造函数，不允许直接调用（只能 new），怎么实现
function Foo() {
  if (!(this instanceof Foo)) {
    throw new Error('error');
  }
}

// 三行布局，header 和 footer 固定高度，content 区域内容不足时依然撑起除 header 和 footer 之外的高度，内容溢出时显示滚动条（使用 flex 如何实现）
```
