# Element Plus ➕ 自动导入 🤖

## 1. [安装 Element Plus ➕](../Element%20Plus%20➕%20安装%20🔧.md)

### npm

```SH
npm install element-plus --save
```

## 2. 安装自动导入插件 🧩

### npm

```SH
npm install -D unplugin-vue-components unplugin-auto-import
```

#### 参考链接

[Element Plus：快速开始｜自动导入](https://element-plus.org/zh-CN/guide/quickstart.html#%E8%87%AA%E5%8A%A8%E5%AF%BC%E5%85%A5-%E6%8E%A8%E8%8D%90)

[unplugin-auto-import](../../../自动导入插件%20🧩/unplugin-auto-import%20🧩.md)

[unplugin-vue-components](../../../自动导入插件%20🧩/unplugin-vue-components%20🧩.md)

## 3. 配置 📝

### Vite

```JS
// vite.config.ts
import { defineConfig } from 'vite'
import AutoImport from 'unplugin-auto-import/vite'
import Components from 'unplugin-vue-components/vite'
import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'

export default defineConfig({
  // ...
  plugins: [
    // ...
    AutoImport({ // 自动导入 JavaScript API @ChatGPT
      resolvers: [ElementPlusResolver()],
    }),
    Components({ // 自动导入 Vue 组件 @ChatGPT
      resolvers: [ElementPlusResolver()],
    }),
  ],
})
```

#### 参考链接

[Element Plus：快速开始｜自动导入｜ Vite](https://element-plus.org/zh-CN/guide/quickstart.html#vite)

---

```JS
AutoImport({
  // Custom resolvers, compatible with `unplugin-vue-components`
  // see https://github.com/antfu/unplugin-auto-import/pull/23/
  resolvers: [
    /* ... */
  ],
})
```

[unplugin-auto-import ｜ Configuration ｜ resolvers](https://github.com/unplugin/unplugin-auto-import?tab=readme-ov-file#configuration)

---

```JS
// vite.config.js
import Components from 'unplugin-vue-components/vite'
import {
  AntDesignVueResolver,
  ElementPlusResolver,
  VantResolver,
} from 'unplugin-vue-components/resolvers'

// your plugin installation
Components({
  resolvers: [
    AntDesignVueResolver(),
    ElementPlusResolver(),
    VantResolver(),
  ],
})
```

[unplugin-vue-components ｜ Importing from UI Libraries](https://github.com/unplugin/unplugin-vue-components?tab=readme-ov-file#importing-from-ui-libraries)
