# fakeUpsShutdown

> It's fake ups shutdown script. Script check to ping router ip address,if router can not be connect,then shutdown system.
这是一个伪装ups关机的脚本。脚本会ping你设置的路由器ip，如果不通会执行关机。

#### 设置说明：
脚本中需要设置三项：
IP: ip地址
sec: 轮循的时间（秒）
count: 允许ping不通几次


#### 设置开机启动：
将脚本加入crontab, @reboot的方式。
