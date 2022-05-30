[TOC]

#### 清空文件
```sh
cat /dev/null > access.log
```


#### 查看空间
```sh
df -h

du -h --max-depth=1
```


#### 查找文件中含有的文字
```sh
grep -rnw '/path/to/somewhere/' -e 'pattern'
```
-r or -R is recursive,
-n is line number, and
-w stands for match the whole word.
-l (lower-case L) can be added to just give the file name of matching files.
-e is the pattern used during the search


#### proxy
```sh
export http_proxy="http://PROXY_SERVER:PORT"
export https_proxy="https://PROXY_SERVER:PORT"
export ftp_proxy="http://PROXY_SERVER:PORT"

export http_proxy="http://USER:PASSWORD@PROXY_SERVER:PORT"
export https_proxy="https://USER:PASSWORD@PROXY_SERVER:PORT"
export ftp_proxy="http://USER:PASSWORD@PROXY_SERVER:PORT"
```


#### .gz
```sh
# 解压缩
# -d 解压 -k 保留源文件
gzip -dk filename.gz
```


#### git
clone 子库
```sh
git submodule update
git submodule init 
```