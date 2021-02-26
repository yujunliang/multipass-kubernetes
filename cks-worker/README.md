#### 3.2 Install worker packages
when in cks-worker,execute the following commands

```
sudo -i
git clone https://github.com/yujunliang/multipass-kubernetes.git
cd multipass-kubernetes/cks-worker
./install-all.sh
```

#### 3.3 Join cks-master as cks-worker

then run what you copied from Step 2, something like this,

```
kubeadm join 192.168.64.3:6443 --token al0kvi.x60mi1xj4zesqnq3     --discovery-token-ca-cert-hash sha256:f4ff0c7684bbac599a8208b94bb28e451023662ab51bc1ce16f60a855a85e2a5
```
