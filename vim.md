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
### Basic
dp  " diff 'put'  
do  " diff 'get'，之所以不用dg，是因为dg已经被另一个命令占用了，所以用了diff 'obtain'

### Other
```vim
:echo 'hello'
:echom 'hello;
" which can be viewed by
:message
```
#### options
```vim
:set showmatch  " for ()[]{} matching
:set matchtime=5  " 0.5s, alias mat matchtime
```
修改后，vimdiff会试图自动来重新比较文件，有时候会处理失败，这个时候就需要手工来刷新。
:diffupdate

