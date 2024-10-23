Deployments Annotations 
------------------------
* Write deployment spec 
* Use killerkoda to deploy the deployment
```sh
kubectl apply -f deploy.yaml
kubectl get all
kubectl get deployments.apps web-deploy 
kubectl rollout history deployment web-deploy
kubectl rollout undo deployment web-deploy
kubectl rollout undo deployment web-deploy --to-revision=<revision number>
```
* ![alt text](images/k8s1.png)
* ![alt text](images/k8s2.png)
* ![alt text](images/k8s3.png)
__change the version to v2 and apply the deployment__
* ![alt text](images/k8s4.png)
* ![alt text](images/k8s5.png)
__change the verison to v3 and apply the deployment__
* ![alt text](images/k8s6.png)
* ![alt text](images/k8s7.png)
__undo rollout to revision no2__
* ![alt text](images/k8s8.png)
* ![alt text](images/k8s9.png)