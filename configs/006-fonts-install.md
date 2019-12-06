# fonts

```shell
# install to user dir
cd ~
mkdir .fonts
cd .fonts
wget https://github.com/afeiship/static-files/raw/master/fonts/Monaco.ttf

# clean cache
fc-cache -vf

# check if installed success:
fc-list | grep Monaca
```
