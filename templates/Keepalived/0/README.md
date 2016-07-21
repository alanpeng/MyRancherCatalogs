# Percona XtraDB Cluster for MySQL Server数据库集群

### 信息：

此模板用于在Rancher里创建一个Percona XtraDB Cluster for MySQL Server。

当你从catalog部署此应用时，一个包含了三节点数据库的集群被创建，你可以预先定义数据库root密码，用户数据库名及密码。集群在三个节点间进行数据同步，属于多活体系。集群节点健康检查服务侦听在8000端口。

### Usage:

当集群部署完毕并运行起来后，使用MySQL客户端进行连接测试：

`mysql -u<db_user> -p -h<pxc>`
例如： `mysql -u wise2c -p -h 172.20.1.10`
