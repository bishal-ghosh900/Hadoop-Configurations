# Hadoop-Configurations

1) **HADOOP-ENV.sh**->>It specifies the environment variables that affect the JDK used by Hadoop Daemon (bin/hadoop). We know that Hadoop framework is wriiten in Java and uses JRE so one of the environment variable in Hadoop Daemons is $Java_Home in Hadoop-env.sh.

2) **CORE-SITE.XML**->>It is one of the important configuration files which is required for runtime environment settings of a Hadoop cluster.It informs Hadoop daemons where the NAMENODE runs in the cluster. It also informs the Name Node as to which IP and ports it should bind.

3) **HDFS-SITE.XML**->>It is one of the important configuration files which is required for runtime environment settings of a Hadoop. It contains the configuration settings for NAMENODE, DATANODE, SECONDARYNODE. It is used to specify default block replication. The actual number of replications can also be specified when the file is created,

4) **MAPRED-SITE.XML**->>It is one of the important configuration files which is required for runtime environment settings of a Hadoop. It contains the configuration settings for MapReduce . In this file, we specify a framework name for MapReduce, by setting the MapReduce.framework.name.

5) **YARN-SITE.XML**->>This file contains the configuration settings related to YARN . For example, it contains settings for Node Manager, Resource Manager, Containers, and Application Master.

6) **Masters**->>It is used to determine the master Nodes in Hadoop cluster. It will inform about the location of SECONDARY NAMENODE to Hadoop Daemon.
The Mater File on Slave node is blank.

7) **Slave**->>It is used to determine the slave Nodes in Hadoop cluster.
The Slave file at Master Node contains a list of hosts, one per line.
The Slave file at Slave server contains IP address of Slave nodes.
