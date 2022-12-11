### 什么是虚拟DOM

### 虚拟 DOM 中 key 的作用

[列表 & Key - React](https://zh-hans.reactjs.org/docs/lists-and-keys.html)

<aside>
💡 key 帮助 React 识别哪些元素改变了，比如被添加或删除。因此你应当给数组中的每一个元素赋予一个确定的标识。`key` 相同的组件，react会判定为相同的组件，所以react利用key来区分组件

如果在React中渲染一个列表，如果没有给列表成员加key属性，react会报一个警告：`a key should be provided for list items`，意思是当你创建一个元素时，必须包括一个特殊的`key`属性。如果没有给列表元素提供key属性时，react内部会自动将index做为key传给列表元素

当渲染一个React列表时，如果只是单纯的展示，key属性的意义不大，反而会因为需要一些diff判断浪费性能

如果一个表列需要做复杂的交互，比如增加、修改、删除，就必须要要加 `key` 属性，并且在同级别列表中是独一无二的字符串，稳定且唯一。不能用随机数，因为每次修改、删除等操作发生时，会发生变化，不稳定

</aside>
