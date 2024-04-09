# Git 📦

## .gitignore 🫥

### [gitignore.io](https://www.toptal.com/developers/gitignore/)

[macOS](https://www.toptal.com/developers/gitignore/api/macos)

### set global user name

```
git config --global user.name "leungsekyu"
```

```
git config user.name
```

### set global user email

```
git config --global user.email "leungsekyu@qq.com"
```

```
git config user.emai
```

### or

```
git config --global --edit
```

```
i
```

```
:wq
```

```
git config --list
```

## [Git Credential Manager 🔑](https://github.com/git-ecosystem/git-credential-manager/blob/main/README.md#git-credential-manager)

### Install

```
brew install --cask git-credential-manager
```

### Upgrade

```
brew upgrade --cask git-credential-manager
```

### Uninstall

```
brew uninstall --cask git-credential-manager
```

[Git Credential Manager：Install instructions](https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/install.md#install-instructions)

## [Oh My Zsh / Git](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git#git-plugin)

| Command                    | Alias |
| :------------------------- | :---- |
| git status                 | gst   |
| git add --all              | gaa   |
| git commit --message       | gcmsg |
| git commit --all --message | gcam  |
| git push                   | gp    |
| git pull                   | gl    |