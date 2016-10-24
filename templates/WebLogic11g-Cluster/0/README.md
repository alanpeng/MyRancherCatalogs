# Oracle WebLogic 11g Cluster
### Info:
This template creates WebLogic server (10.3.6) cluster instances.
### Usage:
Select 'WebLogic11g' from catalog.  Enter the required values in the configuration set. Click Launch. Your application will be ready for access soon from http://your-admin-server-address:8001/console.

One AdminServer with volume mount on local host or NFS shared storage and scalable ManagedServers in one Cluster.

To build your docker image, please modify the username and password of the Oracle website with your own.Please update 2 lines as below in the file "download_jdk6.sh" and "download_weblogic1036.sh":

v_oracle_website_user=peng.alan@gmail.com

v_oracle_website_password=Docker88

Anyway, you can pull the image directly form docker hub as below:

docker pull alanpeng/oracle-weblogic11g-cluster:1036

Default environments for AdminServer:
AdminPort: '8001'
Server_Role: Admin
base_domain_default_password: '999999999'

Default environments for ManagedServer:
AdminPort: '8001'
Server_Role: Managed
base_domain_default_password: '999999999'

Please log in the WebLogic admin console by http://your-admin-server-address:8001 (Username: weblogic   Password: 999999999 )

How ever, you can modify the AdminPort and password with your own. (Managed Server will use the default port 7001).
