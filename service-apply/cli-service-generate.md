
## ClusterIP 서비스 생성
```shell
  kubectl expose deployment yh-app --port=80 --target-port=80 --name=yh-svc-clusterip
```

---

## NodePort 서비스 생성
```shell
    kubectl expose deployment yh-dp --port=8080 --target-port=80 --name=yh-svc-nodeport --type=NodePort
```

## 특정 Pod를 서비스에 노출
```shell
    kubectl expose pod yh-app --port=80 --target-port=80 --name=yh-svc-pod
```

