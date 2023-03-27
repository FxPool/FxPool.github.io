[FxMinerProxy]:https://github.com/FxPool/FXMinerProxy/releases
[Github Release]:https://github.com/FxPool/FXMinerProxy/releases
[image1]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch1-linux-install.png
[image2]:https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/image/tutorial/ch1-linux-run.png
## 1.2 - Linux系统

Linux下FxMinerProxy的搭建
___
### 支持系统
CentOS 7+ / Debian 8+ / Ubuntu 16+ 推荐使用debian系统，需要你系统已经安装curl指令和wget，通常这两个指令已经出厂安装完成，但可能有些厂商也没有安装，手动安装执行命令 
`apt-get update && apt-get install curl && apt-get install wget`
___
### 获取 [FxMinerProxy]
linux系统采用一键脚本自动安装程序无需手动安装，如果你想手动安装可以到[Github Release]下载对应的版本，如果手动安装了程序，后面又想使用脚本安装，可能你需要把之前的安装的程序全部卸载掉，不然可能自动安装脚本不能使用，建议所有操作都通过脚本完成
___
### linux一键安装脚本
```shell
# 下载安装最新版本
bash <(curl -s -L https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/install_zh.sh)
# 下载安装指定版本
bash <(curl -s -L https://raw.githubusercontent.com/FxPool/FXMinerProxy/main/oldversion/install_zh.sh) 版本号(注意这里和前面脚本有一个空格符号)
```
选择1进行安装

![image1]
___
### linux手动安装教程
```shell
# 下载最新安装包
wget https://github.com/FxPool/FXMinerProxy/raw/main/fxminerproxyv3linux.tar.gz
# 解压
tar -zxvf fxminerproxyv3linux.tar.gz
# 进入文件夹
cd fxminerproxyv3linux
# 权限获取
chmod 777 running.sh && chmod 777 fxminerproxyv3
# 执行
setsid ./running.sh &
# 备注可能中间有漏的步骤，请熟悉linux的用户使用，不熟悉的请使用一键安装脚本自动安装
```
___
### 运行 [FxMinerProxy]
按照上面的步骤正常执行，这个时候程序已经正常运行

![image2]

成功执行后会出现账号密码端口，使用你的浏览器，输入`http://你服务器IP:端口`,即可访问后台,端口为控制台表格中打印的PORT项，登录用户名为USER项，密码为PASS项

*__备注:如果浏览器长时间没有响应，请检查你服务器的安全组是否已经开放，首次加载时间可能稍长，请耐心等待__*