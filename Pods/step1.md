`kubectl get pods`{{execute}}
`kubectl run pod1 –generator=run-pod/v1 –image=busybox`{{execute}}
`kubectl get pods`{{execute}}
`kubectl get pod pod1 -o yaml`{{execute}}
`kubectl delete pod pod1`{{execute}}
`kubectl get pods`{{execute}}
