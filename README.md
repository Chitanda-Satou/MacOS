# MacOS

## 好用的软件

```
解压 The Unarchiver
分屏 Spectacle
```

## 软件安装

### 1 iterm2
https://iterm2.com
下载安装

配置参考：
https://www.jianshu.com/p/acfcce731dad

### 2 homebrew
网络条件尚可的前提下，参考：
https://brew.sh
```
cd ~/Downloads
curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install > brew.install
/usr/bin/ruby brew.install
```
替换清华源，参考：
https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/
https://mirrors.tuna.tsinghua.edu.cn/help/homebrew-bottles/

zsh版：
```
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles' >> ~/.zshrc
source ~/.zshrc
```

### 3 VS code
https://code.visualstudio.com/docs/setup/mac
如何添加环境变量也在页面中。

### 4 zsh和oh-my-zsh
```
brew update
brew install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
### 5 lantern下载
https://github.com/getlantern/lantern

### 6 R和Rstudio
MRO:
https://mran.microsoft.com/download
Rstudio：
https://mran.microsoft.com/download

### 
