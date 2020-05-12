# Vim

## Option set

```vim
:set nu!  " toggle bool option
:set nu?  " check any option
:set nonu
```

## Diff

```sh
vimdiff  FILE_LEFT  FILE_RIGHT
# 或者
vim -d  FILE_LEFT  FILE_RIGHT
```

### basic

- dp

    diff 'put'

- do

    diff 'get'，之所以不用 dg，是因为 dg 已经被另一个命令占用了，所以用了 diff 'obtain'

### other

修改后，vimdiff 会试图自动来重新比较文件，有时候会处理失败，这个时候就需要手工来刷新。  
:diffupdate

## Other

### echo

```vim
:echo 'hello'
:echom 'hello;
" which can be viewed by
:message
```

### options

```vim
:set showmatch  " for ()[]{} matching
:set matchtime=5  " 0.5s, alias mat matchtime
```

