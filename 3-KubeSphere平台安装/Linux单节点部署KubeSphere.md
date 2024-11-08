## 1、开通服务器
4c8g；centos7.9；防火墙放行  30000~32767；指定hostname

```bash
hostnamectl set-hostname node1
```

  

## 2、安装
### 1、准备KubeKey
```bash
export KKZONE=cn


curl -sfL https://get-kk.kubesphere.io | VERSION=v1.1.1 sh -

chmod +x kk
```



### 2、使用KubeKey引导安装集群
```bash
#可能需要下面命令
yum install -y conntrack

./kk create cluster --with-kubernetes v1.20.4 --with-kubesphere v3.1.1
```



## 3、安装后开启功能
![image-1730945370195](./assets/image-1730945370195.png)



