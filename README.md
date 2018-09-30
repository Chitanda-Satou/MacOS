# MacOS

## 好用的软件

```
解压 The Unarchiver

分屏 Spectacle

https://www.spectacleapp.com
```

## 软件安装

### 1 iterm2
https://iterm2.com
下载安装

配置参考：
https://www.jianshu.com/p/acfcce731dad


配置rzsz：

https://www.jianshu.com/p/4926a957a41e


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
https://www.rstudio.com/products/rstudio/download/


X11

https://www.xquartz.org

### 7 R包的编译和依赖环境

### 7.1 clang

```
# 报错：
#1
make: /usr/local/clang4/bin/clang: No such file or directory
#2
ld: warning: URGENT: building for OSX, but linking against dylib (/usr/lib/libSystem.dylib) built for (unknown). Note: This will be an error in the future.
#3
1: Setting LC_CTYPE failed, using "C"
2: Setting LC_COLLATE failed, using "C"
3: Setting LC_TIME failed, using "C"
4: Setting LC_MESSAGES failed, using "C"
5: Setting LC_PAPER failed, using "C"

# 解决方案

访问：https://cran.r-project.org/bin/macosx/tools/
下载并安装clang和gfortran

所有的编译依赖问题都可以解决。

```



```
# 报错：


# 解决方案：在shell中运行
Write or paste in: defaults write org.R-project.R force.LANG en_US.UTF-8
```