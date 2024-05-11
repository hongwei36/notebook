### 1. git diff接受的编码格式为utf-8，而文件名是以gb2312格式编写的，所以git diff显示了乱码
```git
git config --global core.quotepath false
```
