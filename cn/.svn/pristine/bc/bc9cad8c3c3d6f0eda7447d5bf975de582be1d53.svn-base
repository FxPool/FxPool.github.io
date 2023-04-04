[image1]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch2-encpage.png
[image2]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-enc-add-apiaddress.png
[image3]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-enc-edit.png
[image4]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-remote-cmd.png
[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues
[SSLMIX配置教程]:https://fxpool.github.io/cn/zh/chapter-7/sslmix-install.html
[image5]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch2-enc-downloadapi.png 
[image6]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch2-edit-enc.png 


## 2.2 - 隧道加密
控制面板-隧道加密
___
![image1]

隧道加密是一种通过加密技术和流量混淆的矿机挖矿连接工具，隧道加密必须在客户的本地电脑或本地的局域网服务器上运行，连接方式
```
矿机(通过stratum+tcp协议)<------>隧道加密软件(通过我们自己开发的加密协议)<------->中转服务器
```
- 加密方式：SSLMIX和 ~~AESMIX~~ 现在只维护sslmix
- API地址：加密客户端通过此API地址连接你的中转服务器
- 在线：显示本地加密客户端个数
- 操作：这里有 ` 下载API配置文件` `执行远程命令` `通知客户端更新连接地址`
- 详细配置请查看[SSLMIX配置教程] 

#### 添加API地址
API地址的目的是加密客户端在启动软件的时候需要连接你的中转服务器然后拉取转发配置，连接建立后中转服务器还可以远程控制加密客户端

<img width="500" src="https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-enc-add-apiaddress.png">

- API端口：随便输入一个不冲突在范围内的端口
- API地址：这里你可输入IP或者域名都可以
- 加密方式：有sslmix aesmix ，aesmix在以后的版本不在维护，老用户可以继续使用
___

#### 下载API配置文件
下载好的API配置文件先保存好一定不要重命名，在[SSLMIX配置教程] 会用到
![image5]
___

#### 编辑加密
<img width="500" src="https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-enc-edit.png">
- 客户端显示的软件名称：你可以自己定义一个名字，此名字将在客户的加密客户端软件启动时显示或访问浏览器显示或者日志显示
- 公告信息：这里你可自己发布一些常用的公告信息，
- 本地转发配置：点击自动生成可以在输入框中自动加载已经配置好的加密端口
___

### 远程通知
当加密客户端在运行的过程中你远程通知将会告诉客户端进行重启拉去最新的配置，所以此功能不要经常使用，每次点击客户端会进行重启大概10s左右完成

![image6]
___

#### 远程命令
可以远程执行linux命令需要知道客户的UUID如果你想远程控制请先记住客户运行的UUID
<img width="500" src="https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-remote-cmd.png">
- 客户端UUID：安装时客户端软件会支持打印到控制台，需要远程控制时要记住
- 指令：只支持linux的命令

> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论