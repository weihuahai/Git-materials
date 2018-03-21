公网、内网是两种Internet的接入方式。
内网接入方式：上网的计算机得到的IP地址是Inetnet上的保留地址，保留地址有如下3种形式：
10.x.x.x
172.16.x.x至172.31.x.x
192.168.x.x
内网的计算机以NAT（网络地址转换）协议，通过一个公共的网关访问Internet。内网的计算机可向Internet上的其他计算机发送连接请求，但Internet上其他的计算机无法向内网的计算机发送连接请求
公网接入方式：上网的计算机得到的IP地址是Inetnet上的非保留地址。公网的计算机和Internet上的其他计算机可随意互相访问。
NAT（Network Address Translator）是网络地址转换，它实现内网的IP地址与公网的地址之间的相互转换，将大量的内网IP地址转换为一个或少量的公网IP地址，减少对公网IP地址的占用。NAT的最典型应用是：在一个局域网内，只需要一台计算机连接上Internet，就可以利用NAT共享Internet连接，使局域网内其他计算机也可以上网。使用NAT协议，局域网内的计算机可以访问Internet上的计算机，但Internet上的计算机无法访问局域网内的计算机。
Windows操作系统的Internet连接共享、sygate、winroute、unix/linux的natd等软件，都是使用NAT协议来共享Internet连接。 所有ISP（Internet服务提供商）提供的内网Internet接入方式，几乎都是基于NAT协议的。