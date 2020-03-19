# nodejs

```shell
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```
## without sudo(failed)
```shell
# pip prepare:
sudo apt-get update
sudo apt-get install python3-pip

echo 'export PATH=$HOME/local/bin:$PATH' >> ~/.bashrc
. ~/.bashrc
mkdir ~/local
mkdir ~/node-latest-install
cd ~/node-latest-install
curl http://nodejs.org/dist/node-latest.tar.gz | tar xz --strip-components=1
./configure --prefix=$HOME/local
make install
curl -L https://www.npmjs.com/install.sh | sh

# node-latest-install 理论上可以删除
```

## resources
- https://stackoverflow.com/questions/31025159/installing-nodejs-without-sudo-in-ubuntu
- https://www.jianshu.com/p/c24de61b4c2d
- https://askubuntu.com/questions/1061486/unable-to-locate-package-python-pip-when-trying-to-install-from-fresh-18-04-in
