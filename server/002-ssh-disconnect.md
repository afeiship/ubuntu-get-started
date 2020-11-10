# ssh
> ssh 经常 卡死 断连 是什么原因

## modify sshd configration
- https://blog.csdn.net/weixin_42591298/article/details/102293350
```shell
cd /etc/ssh
# 备份配置文件
cp sshd_config sshd_config.bak
# 启用客户端活动检查，每60秒检查一次，3次不活动断开连接
sed -i "s/#ClientAliveInterval 0/ClientAliveInterval 60/g" sshd_config
sed -i "s/#ClientAliveCountMax 3/ClientAliveCountMax 3/g" sshd_config
# 确认修改成功
grep ClientAlive sshd_config
# 重新加载ssd配置，让配置生效
service sshd reload
```
