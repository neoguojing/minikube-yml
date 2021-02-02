# 集群版

## 连接

```
命令操作
kubectl  exec -it cassandra-0 -- cqlsh 

集群状态查看
kubectl  exec -it cassandra-0 -- nodetool status 
```
