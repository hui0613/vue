```js
// Vue 构造函数
function Vue(options) {
  // 保证了无法直接通过 Vue() 的形式来调用，只能使用 new 关键字来创建实例
  if (!(this instanceof Vue)) {
    warn("Vue is a constructor and should be called with the `new` keyword");
  }

  this._init(options);
}
```
