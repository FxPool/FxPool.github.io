[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues
[windows]:https://github.com/FxPool/FXMinerProxy/releases
[image1]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-dnx_mb_address.png
[image2]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-ker-dnx.png
[image3]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-hiveos-floghtsheet-dnx.png
[image4]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-hieos-dnx.png
[image5]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-his-select-pool-dnx.png
[image6]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-his-cfg-miner-dnx.png
[image7]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-dnx-portsheet.png
[image8]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch8-dnx-fee.png


## 8.5 - DNX配置说明
控制面板-DNX配置说明
___

#### 配置教程(SRBMiner-MULTI内核)
##### 准备工作
- 1.打开中转后台添加MB纯转发地址地址
![image1]
```shell
# MB官方地址
# 8081端口地址
mallob.neuropool.net:8081
# 443端口地址
dnx.eu.ekapool.com:443
```
- 2.添加一个dnx的矿池转发地址
![image7]

- 3.添加你的抽水信息
你只需要设置你的抽水比例，钱包地址，矿机名，和矿池地址，和其他币种配置一样
![image8]


#### windows配置
- 找到内核bat配置文件`start-mining-dynex.bat`编辑打开
![image2]

```shell
# 这是出厂设置
SRBMiner-MULTI.exe --disable-cpu --algorithm dynex --mallob-endpoint mallob.neuropool.net:8081,https://dnx.eu.ekapool.com --pool dynex.neuropool.net:19331,dnx.eu.ekapool.com:19666 --wallet XwnmPs41nm8D5xdsW6phQbMzZVMWAneRcK6pehVPLDTifKmDQviF1YtTDgnM4X3qjsZrgfgojbnGEZRVepMAQYce28be8WM85 -here
pause
# 修改成如下配置 将8.218.200.46修改成你服务IP
SRBMiner-MULTI.exe --disable-cpu --algorithm dynex --mallob-endpoint 8.218.200.46:8081,8.218.200.46:443 --pool DNX中转地址 --wallet 替换成你的签名名 --pass 矿机名
pause
# 实际例子配置
SRBMiner-MULTI.exe --disable-cpu --algorithm dynex --mallob-endpoint 8.218.200.46:8081,8.218.200.46:443 --pool 8.218.200.46:36320 --wallet XwnuERsfADr9tYwxL8se7sZtiHFZ9JGVCb2ZRkKyJCc6TMfk9mQZY5eTDgnM4X3qjsZrgfgojbnGEZRVepMAQYce28bcwC2pS --pass fxworker
pause
```

#### hiveos配置
创建飞行表选择`SRBMiner-MULTI`内核
![image3]

矿池选择

这里矿池的选择不需要单独设置选择通过内核配置就可以了
![image5]

编辑内核参数
![image6]

配置的参数按照下面的参数填写
![image4]

插件参数
```shell
--disable-cpu --algorithm dynex --mallob-endpoint 8.218.200.46:8081,8.218.200.46:443
```
钱包参数
```shell
%WAL%
```
矿机参数，`这里需要特别注意DNX的矿机名必须是在密码这里，不然矿池显示的是x`
```shell
%WORKER_NAME%
```
中转地址
```shell
直接填写TCP中转地址，比如我这里是 8.218.200.46:36320 
```

#### 总结
- 如果是你自己挖矿那么你按照上面的步骤设置即可
- 如果是连接用户的矿机，那么你需要告诉用户修改两个MB的地址，你可以把上面的教程自己复制修改参数后发给用户
> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论