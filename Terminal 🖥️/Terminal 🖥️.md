# Terminal 🖥️

## [iTerm2](https://iterm2.com/)

## [Oh My Zsh](https://ohmyz.sh/)

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```
open ~/.zshrc
```

```
plugins=(
    git
    zsh-autosuggestions
)
```

```
source ~/.zshrc
```

[zsh-autosuggestions：Installation｜Oh My Zsh](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh)

[freeCodeCamp：如何像专业人士一样使用 Zsh 配置 macOS 终端｜步骤五：更改默认主题｜步骤八：安装插件](https://www.freecodecamp.org/chinese/news/how-to-configure-your-macos-terminal-with-zsh-like-a-pro/)

## [Homebrew 🍺](https://brew.sh/zh-cn/)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## [n 📦](https://github.com/tj/n?tab=readme-ov-file#n--interactively-manage-your-nodejs-versions)

### 安装

```
brew install n
```

[n：Installation｜Third Party Installers](https://github.com/tj/n?tab=readme-ov-file#third-party-installers)

### 获取安装目录的管理员权限

```
# make cache folder (if missing) and take ownership
sudo mkdir -p /usr/local/n
sudo chown -R $(whoami) /usr/local/n
# make sure the required folders exist (safe to execute even if they already exist)
sudo mkdir -p /usr/local/bin /usr/local/lib /usr/local/include /usr/local/share
# take ownership of Node.js install destination folders
sudo chown -R $(whoami) /usr/local/bin /usr/local/lib /usr/local/include /usr/local/share
```

[n：Installation｜1. change the ownership of the relevant directories to yourself (see below)](https://github.com/tj/n?tab=readme-ov-file#installation)

### 安装长期支持版本 Node.js 和 npm

```
n lts
```

[n：Installing Node.js Versions](https://github.com/tj/n?tab=readme-ov-file#installing-nodejs-versions)

### 卸载所有版本 Node.js 和 npm

```
n uninstall
```

[n：Removing Versions](https://github.com/tj/n?tab=readme-ov-file#removing-versions)

---

[npm Docs：Resolving EACCES permissions errors when installing packages globally｜Reinstall npm with a node version manager](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally#reinstall-npm-with-a-node-version-manager)

[npm Docs：Downloading and installing Node.js and npm｜Using a Node version manager to install Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm#using-a-node-version-manager-to-install-nodejs-and-npm)

## [Browsersync 🔗](https://browsersync.io/)

### 安装

```
npm install -g browser-sync
```

### 开始

```
browser-sync start --server --files "**/*"
```

[Stack Overflow：Browser Sync and watching multiple folders](https://stackoverflow.com/questions/36653766/browser-sync-and-watching-multiple-folders)