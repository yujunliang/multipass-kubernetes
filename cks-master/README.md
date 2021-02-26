#### 2.2 Install master packages

when in cks-master VM, execute the following commands

```
sudo -i
git clone https://github.com/yujunliang/multipass-kubernetes.git
cd multipass-kubernetes/cks-master
./install-all.sh
```

#### 2.3 Copy join command

copy the output like this, and prepare to run it in Step 3.3

```
kubeadm join 192.168.64.3:6443 --token al0kvi.x60mi1xj4zesqnq3     --discovery-token-ca-cert-hash sha256:f4ff0c7684bbac599a8208b94bb28e451023662ab51bc1ce16f60a855a85e2a5
```
