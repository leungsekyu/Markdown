# Element Plus ➕ 安装 🔧

## 使用包管理器 📦

### npm

```SH
npm install element-plus --save
```

#### 参考链接

[Element Plus：使用包管理器](https://element-plus.org/zh-CN/guide/installation.html#%E4%BD%BF%E7%94%A8%E5%8C%85%E7%AE%A1%E7%90%86%E5%99%A8)

## 浏览器直接引入

### unpkg

```HTML
<head>
  <!-- Import style -->
  <link rel="stylesheet" href="//unpkg.com/element-plus/dist/index.css" />
  <!-- Import Vue 3 -->
  <script src="//unpkg.com/vue@3"></script>
  <!-- Import component library -->
  <script src="//unpkg.com/element-plus"></script>
</head>
```

#### 参考链接

[Element Plus：浏览器直接引入](https://element-plus.org/zh-CN/guide/installation.html#%E6%B5%8F%E8%A7%88%E5%99%A8%E7%9B%B4%E6%8E%A5%E5%BC%95%E5%85%A5)

### ❗️ 不可以在 DOM 模板里使用自闭合组件 ❗️

```
<ElComponent/> ❌
```

```
<el-component></el-component> ✔️
```

#### 参考链接

[Vue.js 2：风格指南｜自闭合组件](https://v2.cn.vuejs.org/v2/style-guide/#%E8%87%AA%E9%97%AD%E5%90%88%E7%BB%84%E4%BB%B6%E5%BC%BA%E7%83%88%E6%8E%A8%E8%8D%90)
