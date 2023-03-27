[image1]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch2-netswap.png
[image2]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch2-netswap-edit.png
[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues

## 2.3 - 纯转发
控制面板-纯转发
___
![image1]
- 名称：可以任意取一个名
- 端口：随意填写一个本服务器不重的端口
- 地址：目标矿池的地址
___

#### 如何使用SSL/TLS 协议纯转发
- 目标矿池地址不要使用`ssl://`前缀,直接输入目标矿池地址和端口就行，比如目标矿池SSL地址是`stratum+ssl://dnx.sg.ekapool.com:8888`,那么直接填写dnx.sg.ekapool.com:8888
- 矿机端使用stratum+ssl://中转服务器地址:端口
___

#### 如何使用隧道加密纯转发
- 当前版本还不支持，以后会支持
___

#### 编辑添加设置
![image2]


> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论