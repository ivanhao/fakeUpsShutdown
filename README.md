# fakeUpsShutdown

> It's fake ups shutdown script. Script check to ping router ip address,if router can not be connect,then shutdown system. Support `debian9` `debian10` `ProxmoxVE 5` `ProxmoxVE 6` `Openmediavault 4` `Openmediavault 5`
这是一个伪装ups关机的脚本。脚本会ping你设置的路由器ip，如果不通会执行关机。支持`debian9` `debian10` `ProxmoxVE 5` `ProxmoxVE 6` `Openmediavault 4` `Openmediavault 5`

# 一、工具准备

链接：https://github.com/ivanhao/fakeupsshutdown

# 二、安装
###### 方式一：命令行安装

> 需要用root账号来运行

在终端中按行分别执行以下内容：

```
export LC_ALL=C.UTF-8
apt update && apt -y install git && git clone https://github.com/ivanhao/fakeupsshutdown.git
cd fakeupsshutdown
./config
```

###### 方式二：下载zip安装

![download](https://upload-images.jianshu.io/upload_images/4171480-d75f6a4b8d3e7173.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



- 建议使用方式一来安装，不建议直接下载单sh脚本使用，因为那样更新的功能会无法使用！

- 如果网络无法使用，或命令行使用有困难，可以使用方式二下载zip包拷入系统中使用。
然后执行以下命令进行安装配置：
```
./config
```

![main](https://upload-images.jianshu.io/upload_images/4171480-50a64967b0ede749.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

选择install，输入1回车，进行安装。

脚本中需要设置三项：

IP: ip地址

min: 轮循的时间（分）

count: 允许ping不通几次

自动将脚本加入crontab, @reboot的方式，重启后会自动运行。

![steps](https://upload-images.jianshu.io/upload_images/4171480-5670bc8026cb8359.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 三、注意事项

如果将轮询的时间设置过短，会导致ping不通路由的时候开机后马上自动关机，造成不必要的麻烦，请不要将轮询时间设置过短。

如果好用请去github页面点星点赞，

# qq交流群: 878510703

![qq](http://upload-images.jianshu.io/upload_images/4171480-e0204ead0fb41d5e.jpg)

## 如果觉得好的请捐赠一下^_^

![alipay](https://upload-images.jianshu.io/upload_images/4171480-04c3ebb5c11cfdf9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
