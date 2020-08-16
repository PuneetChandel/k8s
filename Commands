# k8s

1. Check Status of cluster
kubectl cluster-info

2. Run Pods
kubectl run nginx → Create Pod, deploy the Ngnix using image from docker hub
kubectl run nginx --image ngnix

3. Create/Update Objects in K8s 
kubectl apply -f client-pod.yaml
kubectl apply -f client-node-port.yaml
- Use deployment file
kubectl apply -f client-deployment.yaml
- To update existing pods, deployments  Change config.yaml → change image name, change replicas etc, use apply command
Kubectl apply -f updated-config-file.yaml

4. Create 
kubectl create -f pod-definition.yml

5. See running objects
kubectl get pods , kubectl get pods -o wide
kubectl get services
kubectl get deployments
kubectl get storageclass
kubectl get nodes

6. Describe objects, detail information
kubectl describe pods client-pod

7. Delete POD
kubectl delete pods <pod>
kubectl delete -f client-pod.yaml
kubectl delete deployment client-deployment
kubectl delete service client-node-port

8. Logs/access container shell etc
kubectl logs <Pod>
kubectl exec -it client-deployment-6854fd9595-4bq4h sh

9. Get detailed info about object
kubectl describe pods client-pod

10. Update using set command
kubectl set image <Type of object>/<objectName> <Container Name> = <new image to use>
kubectl set image deployment/client-deployment client=pchandel/multi-client:v5

11. Create Secret
kubectl create secret generic pgpassword --from-literal PGPASSWORD=12345asdf
