---
draw:
tags: []
title: IP
date created: 2024-09-23
date modified: 2024-12-27
---

相对于[TCP](TCP.md)的面向连接的、可靠的、基于字节流的  
IP协议是无连接的，不可靠的，基于数据报的  
而TCP就像是在这个邮政系统之上增加了跟踪、确认收货、按顺序整理的服务。

## IP数据报

```Java
|--------|--------|--------|--------|              4byte  32bits

    版本      长度          分片长

|--------|--------|--------|--------|    

  片编号     标志            偏移

|--------|--------|--------|--------|    

     TTL      协议           校验码

|--------|--------|--------|--------|    

                   源IP地址

|--------|--------|--------|--------|    

                  目标IP地址

```

## IP地址

[MAC](MAC.md) 地址就像每个人的护照一样，全球唯一，但是与 IP 地址不同，它并没有定位功能。

IP 地址就像一个快递地址一样，是能够直接定位到你的，比如 中国-北京-海淀-维亚大厦-1109

## DHCP

原来配置IP 有这么多门道儿啊。你可能会问了，配置了IP 之后一般不能变的，配置一个服务端的机器还可以，但是如果是客户端的机器呢？我抱着一台笔记本电脑在公司里走来走去，或者白天来晚上走，每次使用都要配置IP 地址，那可怎么办？

还有人事、行政等非技术人员，如果公司所有的电脑都需要IT 人员配置，肯定忙不过来啊。

因此，我们需要有一个自动配置的协议，也就是动态主机配置协议（Dynamic Host Confguration Protocol），简称 DHCP。

有了这个协议，网络管理员就轻松多了。他只需要配置一段*共享的IP地址*。每一台新接入的机器都通过 DHCP 协议，来这个共享的 IP 地址里申请，然后自动配置好就可以了。等人走了，或者用完了，还回去，这样其他的机器也能用。

就好比网络管理员只需要规定『中国-北京-海淀-维亚大厦』就好了至于后面的楼层和工位号，是可以根据 DHCP自动动态生成的。
