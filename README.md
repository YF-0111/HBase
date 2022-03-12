# HBase

bugs and solutions
1. Tables in HBase deleted, but still exist in zookeeper  
    **In Kafka**  
    Check files in zookeeper:  
    > ./zookeeper-shell.sh  node1:2181 ls -R /  
    
    Delete:  
    > ./zookeeper-shell.sh  node1:2181 deleteall  /hbase
    
