# minikube-yml

## minikube

- minikube start --mount-string="/data/minikube:/data" --mount 启动时挂载
- minikube mount /data/minikube:/data 绑定宿主机目录到minikube VM

## PV

- local pv: local:  path: /data/pv ,nodeAffinity 必须配置
- hostpath： "hostPath": "path": "/Users/dalong/pvapp" 必须配置

## 命令

- kubectl describe pod xxx 查看pod日志详细云信情况
- kubectl logs -f xxx  日志

## svc

{服务名}.{namespace}.svc.cluster.local
primary.default.svc.cluster.local
