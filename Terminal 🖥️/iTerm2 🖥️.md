# [iTerm2 🖥️](https://iterm2.com/)

## [Oh My Zsh](https://ohmyz.sh/)

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### [zsh-autosuggestions 🧩](https://github.com/zsh-users/zsh-autosuggestions)

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

#### Reference Link 🔗

[zsh-autosuggestions：Installation ｜ Oh My Zsh](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh)

[freeCodeCamp：如何像专业人士一样使用 Zsh 配置 macOS 终端｜步骤五：更改默认主题｜步骤八：安装插件](https://www.freecodecamp.org/chinese/news/how-to-configure-your-macos-terminal-with-zsh-like-a-pro/)

## [Homebrew 🍺](https://brew.sh/zh-cn/)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## [n 📦](https://github.com/tj/n?tab=readme-ov-file#n--interactively-manage-your-nodejs-versions)

### Why n?

#### Reference Link 🔗

[npm Docs：Resolving EACCES permissions errors when installing packages globally ｜ Reinstall npm with a node version manager](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally#reinstall-npm-with-a-node-version-manager)

[npm Docs：Downloading and installing Node.js and npm ｜ Using a Node version manager to install Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm#using-a-node-version-manager-to-install-nodejs-and-npm)

### Installation

```
brew install n
```

#### Reference Link 🔗

[n：Installation ｜ Third Party Installers](https://github.com/tj/n?tab=readme-ov-file#third-party-installers)

### To take ownership of the system directories

```
# make cache folder (if missing) and take ownership
sudo mkdir -p /usr/local/n
sudo chown -R $(whoami) /usr/local/n
# make sure the required folders exist (safe to execute even if they already exist)
sudo mkdir -p /usr/local/bin /usr/local/lib /usr/local/include /usr/local/share
# take ownership of Node.js install destination folders
sudo chown -R $(whoami) /usr/local/bin /usr/local/lib /usr/local/include /usr/local/share
```

#### Reference Link 🔗

[n：Installation ｜ 1. change the ownership of the relevant directories to yourself (see below)](https://github.com/tj/n?tab=readme-ov-file#installation)

### Install the newest Long Term Support Node.js

```
n lts
```

#### Reference Link 🔗

[n：Installing Node.js Versions](https://github.com/tj/n?tab=readme-ov-file#installing-nodejs-versions)

### Remove all installed Node.js 🗑️

```
n uninstall
```

#### Reference Link 🔗

[n：Removing Versions](https://github.com/tj/n?tab=readme-ov-file#removing-versions)

## [Browsersync](https://browsersync.io/)

### Installation

```
npm install -g browser-sync
```

### Usage

```
browser-sync start --server --files "**/*"
```

#### Reference Link 🔗

[Stack Overflow：Browser Sync and watching multiple folders](https://stackoverflow.com/questions/36653766/browser-sync-and-watching-multiple-folders)
