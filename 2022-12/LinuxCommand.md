1 ## 参看进程监听端口
```
sudo lsof -nP | grep LISTEN | grep 3306
```

2 ## 查看进程号
```
ps -ef | grep 进程名
ps -ef | grep xray
[hong@MacBook] nodebook % ps -ef | grep xray
501  7015     1   0  5:52AM ??         0:53.56 /opt/homebrew/Cellar/xray/1.6.4/libexec/xray run --config /opt/homebrew/etc/xray/config.json
501 73850 73590   0 11:06AM ttys001    0:00.00 grep xray
```

3 ## 查看端口被哪个进程监听
```
sudo lsof -i:8080
```

4 ## 配置git全局变量
```bash
// .gitconfig <--> $XDG_CONFIG_HOME/git/config 
// .gitignore_global <--> $XDG_CONFIG_HOME/git/ignore
mv ~/.gitconfig $XDG_CONFIG_HOME/git/config
mv ~/.gitignore_global $XDG_CONFIG_HOME/git/ignore
```
