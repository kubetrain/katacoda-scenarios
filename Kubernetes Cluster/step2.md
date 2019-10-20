Follow the instructions that given in the Master Node


To start using your cluster, you need to run the following as a regular user:

  `mkdir -p $HOME/.kube`{{execute HOST1}}
  `sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config`{{execute HOST1}}
  `sudo chown $(id -u):$(id -g) $HOME/.kube/config`{{execute HOST1}}
  
  Then you can join any number of worker nodes by running the following on each as root:

Copy "kubeadm join 172.17.0.74:6443 --token 7m2upx.ezqlqe3qhz26baw0"  From the Master
and paste into the node1 then Enter.
