# 05、端口被占用情况解决方案

开始---->运行---->cmd，或者是window+R组合键，调出命令窗口     
查看被占用端口对应的PID，输入命令： `netstat -aon|findstr "49157"` ，回车，记下最后一位数字，即PID,这里是2720。       
关闭对应pid的进程就可以了


mac 处理办法：                           
`sudo lsof -i :port`                                  
`sudo kill -9 pid`
