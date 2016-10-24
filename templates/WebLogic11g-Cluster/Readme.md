# Oracle-Weblogic11g-Cluster-Rancher-Catalog
Oracle WebLogic 11g version 1036 Dockerfile for cluster deployment on Rancher.

One Admin Server with volume mount on local host or NFS shared storage.
Scalable Managed Servers in one Cluster.

To build your docker image, please modify the username and password of the Oracle website with your own.
Please update 2 lines as below in the file "download_jdk6.sh" and "download_weblogic1036.sh

"v_oracle_website_user=peng.alan@gmail.com

v_oracle_website_password=Docker88

Anyway, you can pull the image directly form docker hub as below:

docker pull alanpeng/oracle-weblogic11g-cluster:1036

