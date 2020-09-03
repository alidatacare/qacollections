1.启动zk
2.启动journalnode:
        hadoop-daemons.sh start journalnode
3.格式化zkfc--让在zookeeper中生成ha节点
        hdfs zkfc –formatZK
4.格式化hdfs
        hadoop namenode –format
5.启动NameNode
        hadoop-daemon start namenode
6.standby同步namenode的数据，并启动
        hdfs namenode –bootstrapStandby
7.启动启动datanode
        hadoop-daemons.sh start datanode
8.启动yarn
        sbin/start-yarn.sh
9.启动zkfc
        hadoop-daemons.sh start zkfc



1. hadoop namenode -format
2. start-dfs.sh 



文件系统的基本操作：hadoop fs -help可以获取所有的命令及其解释

常用的有：

hadoop fs -ls /   列出hdfs文件系统根目录下的目录和文件
hadoop fs -copyFromLocal <local path> <hdfs path> 从本地文件系统将一个文件复制到HDFS
hadoop fs -rm -r <hdfs dir or file> 删除文件或文件夹及文件夹下的文件
hadoop fs -mkdir <hdfs dir>在hdfs中新建文件夹
HDFS的文件访问权限：只读权限（r），写入权限（w），可执行权限（x）

日志
http://node01:50070/logs/

浏览器
http://node01:50070/explorer.html#/
