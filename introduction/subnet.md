# VPC和子网简介

## VPC

私有网络 VPC（Virtual Private
Cloud）是属于用户的、逻辑隔离的网络环境。在私有网络中，可以创建指定网段的VPC，在VPC中创建子网并自主管理云资源。创建VPC时，可自主规划网段，灵活为VPC指定网段。目前VPC支持的网段范围如下：

  - 10.0.0.0/8（10.0.0.0-10.255.255.255）掩码范围：最大为 /8 掩码，最小为 /29 掩码。
  - 172.16.0.0/12（172.16.0.0-172.31.255.255）掩码范围：最大为 /12 掩码，最小为 /29 掩码。
  - 192.168.0.0/16（192.168.0.0-192.168.255.255）掩码范围：最大为 /16 掩码，最小为 /29
    掩码。
    
> 默认VPC不支持新增网段，[详情](https://docs.ucloud.cn/vpc/configurationguide/vpcguide?id=_1%ef%bc%8c%e5%90%8d%e7%a7%b0%e8%a7%a3%e9%87%8a)。

## 子网

为了科学有效地划分VPC内的地址空间，将其划分为更细粒度的网络段。这些独立的网络段叫做子网（Subnet）。

子网内云资源支持跨可用区部署，为跨可用区灾备提供有力保障。

子网网段的掩码最小为/29掩码。当子网中有云资源时，该子网不允许删除。

在各地域我们会创建默认VPC和默认子网，用户可直接将云资源创建在默认VPC中。

## VPC网络互通

同一VPC内网络默认互通，不同VPC间网络默认不通。VPC网络互通功能可实现不同项目／不同地域的VPC间网络互通，其中不同地域间的VPC需要互通时，需要[高速通道](udpn/README)配合使用。

互通的VPC间网段不允许重叠。详细关于VPC网络互通的能力见[VPC联通规则](https://docs.ucloud.cn/vpc/configurationguide/vpcguide?id=vpc%e8%81%94%e9%80%9a%e8%a7%84%e5%88%99)。

## 产品配额

每个账号默认配额如下

| 名称         | 配额  |
| ---------- | --- |
| 每个地域的VPC数量 | 100 |
| 每个VPC的子网数量 | 200 |
