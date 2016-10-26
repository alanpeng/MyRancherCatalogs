# Get Loadbalancer Host IP

### 信息：

此模板用于在Rancher里为某种特殊场景的需求，取回HA-Proxy负载均衡所在宿主机IP地址给Web容器。这里负载均衡有多个，因此取回的IP是Keepalived的VIP，将其由Web容器返回给SSO单点登录服务器。

### 使用方法:

在创建该Catalog应用时，请特别注意宿主机网卡名，例如有可能是`eth0`，也有可能是`eno16777984`这样的格式。
当集群部署完毕并运行起来后，使用在Catalog中定义好的虚拟IP地址及侦听端口访问应用。

`http://<Virtual IP>:<port>`
例如：`http://172.18.1.68:3000`
