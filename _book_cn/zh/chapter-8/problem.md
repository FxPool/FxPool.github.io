[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues
[纯转发(开源)]:https://github.com/snail007/goproxy

## 8.1 - 常见问题
控制面板-常见问题FAQ
___

#### Q：软件安装失败这么办？
> A：如果出现permission denied 说明当前你不是root权限需要进去root权限 debian，unbantu，执行 su 命令 输入密码即可

___

#### Q：软件安装成功浏览器打不开？
> A：这种问题一般是端口没有开放，如果你购买的云服务器比如阿里等需要首先到云服务器后台开放端口安全组，使用什么端口就开放什么
>端口，也可以全部开放范围0-65535.然后如果还是连接不上，且系统是linux的话还需要开放服务器的端口。服务器可以直接关闭防火
>墙。使用 ufw disable(debian和unbantu系统)。

___

#### Q：抽水转换率过大的问题？
> A：由于芯片机器不提交算力，fxminerproxy是根据难度动态计算，10分钟计算一次所以芯片机要等10分钟后才能显示，算力只做参考具体
以矿池为准

___

#### 本地矿机已经连接上了但是后台不显示？
> A：fxminerproxy需要矿机成功提交一次有效的份额才会显示，请等待矿机提交有效的份额

___

#### 是否支持专业机器(芯片机)？
> A：程序的端口会自动判断是显卡机器还是芯片机器所以无效单独配置 A11矿机抽水最好是抽到相同的矿池，不同的矿池可能会出现无效，主
>要还是要看固件是否支持set_exnaoce方法(动态修改随机数)，保守做法抽到同一个矿池 奶牛、茉莉、亚米等矿机可抽任意矿池 **自己定义
>目标矿池的问题,fxminerProxy支持自定义端口，有小伙伴经常问到为什么只能下拉选择不能自己输入，其实输入和下拉是做到一起的，鼠标选
>中后直接输入回车确定即可

___

#### 不开抽水功能是否真的作者不抽水？
> A：这个问题其实容易测试，可以用纯转发的软件测试对比算力。纯转发软件可以用这个[纯转发(开源)]

___


> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论