# 集群版

## 连接

kubectl  exec -it redis-app-0 -- redis-cli 

## 集群初始化

```
kubectl exec -it redis-app-0 -- redis-cli --cluster create --cluster-replicas 1 \
$(kubectl get pods -l app=redis-cluster-app -o jsonpath='{range.items[*]}{.status.podIP}{":6379 "}{end}') 
```

## 说明
pv-local.yaml 不支持minikube
