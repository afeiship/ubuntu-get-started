# rime

```shell
# input
sudo apt-get install ibus-rime

# wubi data source
sudo apt-get install librime-data-wubi
```
## config
```yaml
# ~/.config/ibus/rime/default.yaml

schema_list:   
  - schema: luna_pinyin_simp #simp是简体，第一位是默认输入法 
menu:
  page_size: 9 #每页候选词个数
ascii_composer:
  switch_key:
    Shift_L: commit_code #左shift提交字母
```

## resources
- https://github.com/rime/home/wiki/RimeWithIBus
- https://www.jianshu.com/p/4793e55751ec
- https://www.jianshu.com/p/67265175357e
