# wxMD5

微信小程序 JavaScript MD5 实现。

## 使用方法

1. 下载 md5.js 到项目中
2. 全局或局部引入：`import md5 from 'path/to/md5.js'`

## API

> 大部分时候，你只会用到前两种。如果不确定第2到4种的用法，建议用第一种即可

1. 给定一个字符串，计算得出它的 MD5 哈希值

```js
var hash = md5('value') // "2063c1608d6e0baf80249c42e2be5804"
```

2. 给定一个字符串，计算得出它的 [HMAC-MD5](https://www.zhihu.com/question/19816240) 哈希值

```js
var hash = md5("value", "key") // "01433efd5f16327ea4b31144572c67f6"
```

3. Calculate the raw MD5 hash of a given string value

```js
var hash = md5("value", null, true)
```

4. Calculate the raw HMAC-MD5 hash of a given string value and key

```js
var hash = md5("value", "key", true)
```

## 感谢

JavaScript-MD5 [![GitHub stars](https://img.shields.io/github/stars/blueimp/JavaScript-MD5.svg?style=social&label=Stars)](https://github.com/blueimp/JavaScript-MD5)：JavaScript MD5 implementation. Compatible with server-side environments like node.js, module loaders like RequireJS and all web browsers. 官网：https://blueimp.github.io/JavaScript-MD5/
