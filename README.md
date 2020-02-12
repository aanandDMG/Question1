# goals101Jenkins


Requirements

Kubernetes

---------------------------------------------------------------------------------------------------------------
Details
---------------------------------------------------------------------------------------------------------------

1. Kindly create this path /var/lib/jenkins/workspace by mkdir.

2. Kindly run pv.yaml by kubectl apply -f pv.yaml. It will create a PersistentVolume.

3. Once second step is done kindly run kubectl apply -f pvc.yaml, it will create PersistentVolumeClaim.

4. At final step kindly run kubectl apply -f jenkins.yaml, this will create deployment for the Jenkins having 3 replicas and attaching PVC accordingly.

kindly verify pv & pvc by:

kubectl get pv
kubectl get pvc

Deployment and description can be checked by:

kubectl get deployment
kubectl describe depolyment jenkins 
