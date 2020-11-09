# initialize
> 装机必备.

## change source
- https://github.com/afeiship/ushell-module-ubuntu-sources
```shell
# 1. backup old
cp /etc/apt/sources.list /etc/apt/sources.list.bak

# 2. use new 
vim /etc/apt/sources.list

# 3. udpate
apt-get update && apt-get upgrade
```

> 阿里云的源
~~~
deb http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse
~~~


## dotfiles
```shell
# install dotfiles
cd ~
git clone https://github.com/afeiship/dotfiles.git .dotfiles
./.dotfiles/bin/dfm install


## when met bad permission
cd ~/.ssh
chmod 600 ~/.ssh/id_rsa
chmod 600 *.*
```

## nodejs
- https://github.com/afeiship/ubuntu-nodejs-install

```shell
## install
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo apt-get install -y nodejs

## check:
node -v
npm -v
```

## ubuntu-settings
- https://github.com/afeiship/ubuntu-settings

```shell
# 1. clone project
cd ~/github
git clone git@github.com:afeiship/ubuntu-settings.git

# 2. install dependencies
cd ubuntu-settings
npm i -S @afeipship/ushell-module-secret --registry=https://npm.pkg.github.com

# 3. install common packages
npm i --registry=https://registry.npm.taobao.org
```

## autojump
```shell
apt install autojump
```
