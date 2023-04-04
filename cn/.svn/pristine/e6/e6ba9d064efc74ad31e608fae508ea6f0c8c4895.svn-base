[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues
[FxMinerProxy]:https://github.com/FxPool/FXMinerProxy

## 8.3 - 关于算力
控制面板-关于算力
___

#### [FxMinerProxy]计算算力的原理如下
如果矿机本身上报算力比如ETC等显卡矿机那么[FxMinerProxy]会直接显示矿机上报的算力，若没有上报算力，则每10分钟统计一次份额通过矿池下发的难度动态计算算力，这样做如果矿池的难度是不变化的
那么计算的算力则和矿池一样，如果矿池的难度是变化的则计算的算力是不准确的，我们后面会研究如何计算动态难度矿池的算力，请再等等。
###### 计算的公式
```
算力=10分钟有效份额数/600*难度
```


> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论