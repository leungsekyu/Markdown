# Vue 🖼️

### 对动态参数表达式的约束

在 DOM 中使用模板时 (直接在一个 HTML 文件里撰写模板)，还需要**避免使用大写字符来命名键名**，因为浏览器会把 attribute 名**全部强制转为小写**：

```
<!--
在 DOM 中使用模板时这段代码会被转换为 `v-bind:[someattr]`。
除非在实例中有一个名为“someattr”的 property，否则代码不会工作。
-->
<a v-bind:[someAttr]="value"> ... </a>
```

[Vue.js 2：模板语法｜动态参数｜对动态参数表达式的约束](https://v2.cn.vuejs.org/v2/guide/syntax.html#%E5%8A%A8%E6%80%81%E5%8F%82%E6%95%B0)

### 使用一个对象绑定多个 prop

如果你想要将一个对象的所有属性都当作 props 传入，你可以**使用没有参数的 v-bind**，即只使用 v-bind 而非 :prop-name。

```
const post = {
  id: 1,
  title: 'My Journey with Vue'
}
```

```
<BlogPost v-bind="post" />
```

[Vue.js 3：Props ｜使用一个对象绑定多个 prop](https://cn.vuejs.org/guide/components/props#binding-multiple-properties-using-an-object)  
[Vue.js 3：模板语法｜动态绑定多个值](https://cn.vuejs.org/guide/essentials/template-syntax.html#dynamically-binding-multiple-attributes)

## data

**组件的 `data` 必须是一个函数。**

[Vue.js 2：风格指南｜组件数据](https://v2.cn.vuejs.org/v2/style-guide/#%E7%BB%84%E4%BB%B6%E6%95%B0%E6%8D%AE%E5%BF%85%E8%A6%81)  
[Vue.js 3：选项式 API ｜状态选项｜ data](https://cn.vuejs.org/api/options-state.html#data)

## 组件

未声明传参会挂载到 template 根节点 ✍🏻

## 事件

### @input

[MDN：HTML 元素｜ input 事件](https://developer.mozilla.org/zh-CN/docs/Web/API/Element/input_event)

### @change

[MDN：HTML 元素｜ change 事件](https://developer.mozilla.org/zh-CN/docs/Web/API/HTMLElement/change_event)

## 响应式 API

### ref()

ref()：接受一个内部值，返回一个响应式的、可更改的 ref 对象，此对象只有一个指向其内部值的属性 `.value`。

[Vue.js 3：响应式基础｜ ref()](https://cn.vuejs.org/guide/essentials/reactivity-fundamentals.html#ref)
