# Shanghai-Telecom-IPTV
将vlan85 作为access开放给ikuai的额外wan口，该wan口开启DHCP 
确定对应Wan*口获取到IP后设置IGMP代理，网络设置---IGMP代理  ：勾选开启。上联口选取对应的IPTV wan 下联口选LAN
高级应用---UDPXY：   添加信号源- wan*,  服务端口：5146（任意端口都可以）。

找到对应的igmp地址修改成   http://*.*.*.*:5146/udp/x.x.x.x:5146     前面的*.*.*.* 代表路由器地址     x.x.x.x代表直播源地址
