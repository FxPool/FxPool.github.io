[homeicon]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/home-en.png
[Telegram 讨论群组]:https://t.me/FxminerChat
[问题讨论]:https://github.com/FxPool/FXMinerProxy/issues
[SSLMIX]:https://github.com/FxPool/SSLMIX/releases
[SSLMIX Windows系统]:https://github.com/FxPool/SSLMIX/raw/main/ssmixwindows.zip
[Github Release]:https://github.com/FxPool/SSLMIX/releases
[image1]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-sslmix-install.png
[image2]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-sslmix-firstrun.png
[image3]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-sslmix-upload-apifile.png
[image4]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-run-succ.png
[image5]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch7-worker-conn-address.png


## 7.6 - SSLMIX安装配置

SSLMIX的搭建教程
___
### 支持系统
windows和linux，支持架构包括 
`windows8以上所有32位64位系统` 

`linux amd64架构` 

`linux arm32 v7 (armv7l)架构`

___
### 获取 [SSLMIX]
* windows系统
> 直接下载解压运行即可 [SSLMIX Windows系统]

* Linux 系统
> linux系统采用一键脚本自动安装程序无需手动安装，如果你想手动安装可以到[Github Release]下载对应的版本，如果手动安装了程序，后面又想使用脚本安装，可能你需要把之前的安装的程序全部卸载掉，不然可能自动安装脚本不能使用，建议所有操作都通过脚本完成

___
### linux一键安装脚本
国际网络
```shell
# 一键安装脚本(linux amd64架构)
bash <(curl -s -L https://raw.githubusercontent.com/FxPool/SSLMIX/main/install_zh.sh) https://raw.githubusercontent.com/FxPool/SSLMIX/main ssmixlinux
# 一键安装脚本(linux arm32 v7 (armv7l)架构)
bash <(curl -s -L https://raw.githubusercontent.com/FxPool/SSLMIX/main/install_zh.sh) https://raw.githubusercontent.com/FxPool/SSLMIX/main ssmixlinux32armv7l
```
中国大陆网络
```shell
# 一键安装脚本(linux amd64架构)
bash <(curl -s -L https://cdn.jsdelivr.net/gh/FxPool/SSLMIX/install_zh.sh) https://cdn.jsdelivr.net/gh/FxPool/SSLMIX@main ssmixlinux

# 一键安装脚本(linux arm32 v7 (armv7l)架构)
bash <(curl -s -L https://cdn.jsdelivr.net/gh/FxPool/SSLMIX/install_zh.sh) https://cdn.jsdelivr.net/gh/FxPool/SSLMIX@main ssmixlinux32armv7l

```
选择1进行安装

![image1]
___
### linux手动安装教程
```shell
# 下载最新安装包 这里选择amd64架构的包 arm架构安装一样
wget https://github.com/FxPool/SSLMIX/raw/main/ssmixlinux.tar.gz
# 解压
tar -zxvf ssmixlinux.tar.gz
# 进入文件夹
cd ssmixlinux
# 权限获取
chmod 777 running && chmod 777 sslmix
# 执行
setsid ./running &
# 备注可能中间有漏的步骤，请熟悉linux的用户使用，不熟悉的请使用一键安装脚本自动安装
```
___
### 运行 [SSLMIX]
按照上面的步骤正常执行，首次运行会出现叫你上传API配置文件，如果你的后台已经添加了对应的API地址，请下载api配置文件上传到sslmix软件，`不要重命名`

![image2]

输入`http://127.0.0.1:62440`进入web管理后台,在`设置`界面点击`选择配置文件`然后点击`上传api配置文件`,上传成功后需要重启软件才能生效

![image3]

运行成功后会在控制台打印出你配置的端口信息

![image4]

网页后台也能查看配置的信息

![image5]


> 复杂的问题可以进[Telegram 讨论群组]， 常用疑问可以通过[问题讨论]查看或自己创建问题大家讨论