# unplugin-icons 🧩

Access thousands of icons as components on-demand universally.

## Installation

### npm

```SH
npm i -D unplugin-icons
```

#### Reference Link

[unplugin-icons：Install ｜ Plugin](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#plugin)

## Configuration

### Vite

```JS
// vite.config.ts
import Icons from 'unplugin-icons/vite'

export default defineConfig({
  plugins: [
    Icons({ /* options */ }),
  ],
})
```

#### Reference Link

[unplugin-icons：Configuration ｜ Vite](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#plugin)

## Auto Importing

### Vue 2 & 3

Use with [unplugin-vue-components](https://github.com/antfu/unplugin-vue-components)

```JS
// vite.config.js
import Vue from '@vitejs/plugin-vue'
import Icons from 'unplugin-icons/vite'
import IconsResolver from 'unplugin-icons/resolver'
import Components from 'unplugin-vue-components/vite'

export default {
  plugins: [
    Vue(),
    Components({
      resolvers: [
        IconsResolver(),
      ],
    }),
    Icons(),
  ],
}
```

### Name Conversion

When using ==component resolver==, you have to follow the name conversion for icons to be properly inferred.

```HTML
<{prefix}-{collection}-{icon} />
```

By default, the prefix is set to `i`

```HTML
<i-{collection}-{icon} /> ❗️
```

The `collection` field follows [Iconify's collection IDs](https://icon-sets.iconify.design/)

#### Reference Link

[unplugin-icons：Auto Importing ｜ Vue 2 & 3](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#auto-importing)

[unplugin-icons：Auto Importing ｜ Name Conversion](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#name-conversion)

## Icons Data Auto Installation ( [Iconify](https://iconify.design/) )

### Vite

```JS
Icons({
  // experimental
  autoInstall: true,
})
```

#### Reference Link

[unplugin-icons：Install ｜ Icons Data ｜ autoInstall
](https://github.com/unplugin/unplugin-icons?tab=readme-ov-file#icons-data)
