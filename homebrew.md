# [Homebrew](https://brew.sh/)

**不要折腾手动编译了，很多东西很麻烦**

**比如万恶的openssl、pkg-config、cmake，老老实实用`brew`，臃肿就臃肿一点吧😂**

## 安装 & 镜像源

中科大源

**不要用清华tuna的源，会限速！！！**

```shell
export HOMEBREW_BREW_GIT_REMOTE="https://mirrors.ustc.edu.cn/brew.git"
export HOMEBREW_CORE_GIT_REMOTE="https://mirrors.ustc.edu.cn/homebrew-core.git"
export HOMEBREW_BOTTLE_DOMAIN="https://mirrors.ustc.edu.cn/homebrew-bottles"
```

然后按照[官网](https://brew.sh/)的说明安装即可

```shell
# 官网
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 修改一下快速安装
sudo mkdir /opt/homebrew && sudo chown -R xxx:admin /opt/homebrew && \
git clone --depth 1 https://github.com/Homebrew/brew /opt/homebrew && \
eval "$(/opt/homebrew/bin/brew shellenv)"

```

## 卸载方法

[官网说明](https://github.com/homebrew/install#uninstall-homebrew)

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"
```
