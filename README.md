# fakeUpsShutdown

> It's fake ups shutdown script. Script check to ping router ip address,if router can not be connect,then shutdown system.
这是一个伪装ups关机的脚本。脚本会ping你设置的路由器ip，如果不通会执行关机。

#### 一、设置说明：
```
./config
```

选择install进行安装。

脚本中需要设置三项：

IP: ip地址

min: 轮循的时间（分）

count: 允许ping不通几次


#### 二、设置开机启动：
用./config进行安装，会自动将脚本加入crontab, @reboot的方式。


#### 三、注意事项

如果将轮询的时间设置过短，会导致ping不通路由的时候开机后马上自动关机，造成不必要的麻烦，请不要将轮询时间设置过短。
