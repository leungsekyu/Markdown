# Vue 自动导入 👨🏻‍💻

## Node.js

```
required: { node: '^18.0.0 || >=20.0.0' }
```

[Node.js：Downloads](https://nodejs.org/en/download/)

## Element Plus

```
npm install element-plus --save
npm install @element-plus/icons-vue
npm install -D unplugin-vue-components unplugin-auto-import
npm i -D unplugin-icons
```

[Element Plus：使用包管理器](https://element-plus.org/zh-CN/guide/installation.html#%E4%BD%BF%E7%94%A8%E5%8C%85%E7%AE%A1%E7%90%86%E5%99%A8)  
[Element Plus：Icon 图标｜使用包管理器](https://element-plus.org/zh-CN/component/icon.html#%E4%BD%BF%E7%94%A8%E5%8C%85%E7%AE%A1%E7%90%86%E5%99%A8)  
[Element Plus：自动导入](https://element-plus.org/zh-CN/guide/quickstart.html#%E8%87%AA%E5%8A%A8%E5%AF%BC%E5%85%A5-%E6%8E%A8%E8%8D%90)  
[unplugin-icons：Install｜Plugin](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#plugin)

## vite.config.ts / vite.config.js

```
import AutoImport from 'unplugin-auto-import/vite'
import Components from 'unplugin-vue-components/vite'
import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'

import Icons from 'unplugin-icons/vite'
import IconsResolver from 'unplugin-icons/resolver'
```

```
AutoImport({
  imports: ['vue', 'vue-router'],

  resolvers: [ElementPlusResolver()],
}),

Components({
  resolvers: [ElementPlusResolver(), IconsResolver()],
}),

Icons({
  autoInstall: true,
}),
```

[Element Plus：自动导入｜Vite](https://element-plus.org/zh-CN/guide/quickstart.html#vite)  
[Element Plus：Icon 图标｜自动导入](https://element-plus.org/zh-CN/component/icon.html#%E8%87%AA%E5%8A%A8%E5%AF%BC%E5%85%A5)  
[unplugin-icons：Auto Importing｜Vue 2 & 3](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#auto-importing)     
[unplugin-auto-import：Configuration](https://github.com/unplugin/unplugin-auto-import?tab=readme-ov-file#configuration)

## 用法

```
<i-{collection}-{icon} />
```

[unplugin-icons：Name Conversion](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#name-conversion)  
[Element Plus：图标集合](https://element-plus.org/zh-CN/component/icon.html#icon-collection)  
[iconify：Icons](https://icon-sets.iconify.design/)