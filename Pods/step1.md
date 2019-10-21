A Pod is the basic execution unit of a Kubernetes object model that you create or deploy.
It represents processes running on your Cluster.
It might contain single or multiple containers.
Each Pod is meant to run a single instance of a given application. 
CREATION
`nano po-kubetrain.yaml`{{execute}}
<pre class="file" data-filename="po-kubetrain.yaml" data-target="replace">
apiVersion: v1
kind: Pod
metadata:
  name: po-kubetrain
spec:
  containers:
  - name: ctr-kubetrain
    image: httpd
</pre>
`kubectl get pods`{{execute}}
`kubectl run pod1 –generator=run-pod/v1 –image=nginx`{{execute}}
`kubectl get pods`{{execute}}
`kubectl get pod pod1 -o yaml`{{execute}}
`kubectl delete pod pod1`{{execute}}
`kubectl get pods`{{execute}}
