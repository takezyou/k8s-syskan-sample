https://kubernetes.io/ja/docs/tasks/run-application/run-single-instance-stateful-application/

```
$ kubectl apply -f mysql-pv.yaml
$ kubectl apply -f mysql-deployment.yaml
$ kubectl describe deployment mysql
$ kubectl get pods -l app=mysql
$ kubectl describe pvc mysql-pv-claim
$ kubectl run -it --rm --image=mysql:5.6 --restart=Never mysql-client -- mysql -h mysql -ppassword
```
