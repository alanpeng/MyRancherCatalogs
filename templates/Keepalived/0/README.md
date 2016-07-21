# Keepalived for Rancher HA-Proxy Loadbalancer

### 信息：

此模板用于在Rancher里内置的基于HA-Proxy技术的多个LoadBalancer节点创建一个Failover高可用服务。

当你从catalog部署此应用时，一个全局（global）的集群被创建，因此你可以在创建此Catalog时先不启动它，创建之后利用Host Lable来设置容器调度策略，以确保此HA应用运行在适合的宿主机上。

### Usage:

当集群部署完毕并运行起来后，使用在Catalog中定义好的虚拟IP地址及侦听端口访问应用。

`http://<Virtual IP>:<port>`
例如：`http://172.18.1.68:3000`
