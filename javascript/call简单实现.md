```js
Function.prototype.call2 = function(context) {
  var context = context || window; //因为传进来的context有可能是null
  context.fn = this;
  var args = [];
  for (var i = 1; i < arguments.length; i++) {
    args.push("arguments[" + i + "]"); //不这么做的话 字符串的引号会被自动去掉 变成了变量 导致报错
  }
  args = args.join(",");

  var result = eval("context.fn(" + args + ")"); //相当于执行了context.fn(arguments[1], arguments[2]);

  delete context.fn;
  return result; //因为有可能this函数会有返回值return
}
// or
Function.prototype.myCall = function(context) {
  if (typeof this !== 'function') {
    throw new TypeError('Error')
  }
  /**
   * a.call(b, 2)
   * context = b
   * this = function myCall () { .... }
   * context.fn = b.fn
   */
  context = context || window
  context.fn = this
  const args = [...arguments].slice(1)
  const result = context.fn(...args)
  delete context.fn
  return result
}
```