# Kubernetes Vagrant Lab

## Khởi động Master Node

```bash
vagrant up k8s-master
```
## Lấy file joincluster.sh
```bash
vagrant scp k8s-master:/joincluster.sh .
```
## Khởi động Worker Node
```bash
vagrant up k8s-worker-1
```
## Kiểm tra cụm Kubernetes
```bash
vagrant ssh k8s-master
kubectl get nodes -o wide
kubectl get pods -A -o wide
````