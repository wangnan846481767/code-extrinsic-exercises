# 工程乱码

打开File-Setting, 找到File Encodings这个选项，把encoding设置成你工程的编码即可，一般是UTF-8，如下图（红框的地方），然后重新rebuild一下，基本就行了
![title](https://raw.githubusercontent.com/wangnan846481767/gitnote-images/master/2019/06/20/20180618122110880-1560999324348.png)
# 执行main函数时，控制台乱码

同样是打开setting，找到 Build,Execution,Deployment > Compiler > Java Compiler， 设置 Additional command line parameters选项为 -encoding utf-8，然后rebuild下，重新运行

![title](https://raw.githubusercontent.com/wangnan846481767/gitnote-images/master/2019/06/20/20180618122329161-1560999339029.png)

# 运行tomcat时，控制台乱码
1. 打开Run/Debug Configuration,选择你的tomcat
	![title](https://raw.githubusercontent.com/wangnan846481767/gitnote-images/master/2019/06/20/20180618122616180-1560999390661.png)
2. 然后在 Server > VM options 设置为 -Dfile.encoding=UTF-8 ，重启tomcat
 	![title](https://raw.githubusercontent.com/wangnan846481767/gitnote-images/master/2019/06/20/20180618122645199-1560999406638.png)