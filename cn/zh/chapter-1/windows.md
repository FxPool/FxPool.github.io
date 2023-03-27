[FxMinerProxy]:https://github.com/FxPool/FXMinerProxy/releases
[Github Release]:https://github.com/FxPool/FXMinerProxy/releases
## 1.1 - Windows系统

Windows下FxMinerProxy的搭建
___
### 支持系统
 Windows8以上版本都支持,推荐使用windows server 2012
___
### 获取 [FxMinerProxy]
请到 [Github Release] 下载最新的版本，下载老版本选择对应的版本号即可，windows系统的命名为fxminerproxyv3windows.zip
___
### 运行 [FxMinerProxy]
使用zip解压工具，直接解压zip压缩包,选择全部提取

<img width="400" src="https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch1-windows.png">

然后运行run.exe可执行文件，run.exe是守护进程可以保证程序用不死机

<img width="700" src="https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch1-windows-run.png">

成功执行后会出现账号密码端口，使用你的浏览器，输入`http://你服务器IP:端口`,即可访问后台,端口为控制台表格中打印的PORT项，登录用户名为USER项，密码为PASS项

*__备注:如果浏览器长时间没有响应，请检查你服务器的安全组是否已经开放，首次加载时间可能稍长，请耐心等待__*