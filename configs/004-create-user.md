# create user

## steps
```shell
sudo adduser feizheng

# chekc
cat /etc/passwd
grep '^feizheng' /etc/passwd

# feizheng:x:1000:1000:afei,,,:/home/feizheng:/bin/bash
```

## sudo list
```shell
# [error]: feizheng is not in the sudoers file.  This incident will be reported.

```

## resources
- https://www.cyberciti.biz/faq/create-a-user-account-on-ubuntu-linux/
- https://blog.csdn.net/jiangjiang_jian/article/details/81169258
