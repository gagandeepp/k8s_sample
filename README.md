kubectl create -f pod-definition.yaml \
kubectl get pods -o wide \
kubectl describe pod myapp-pod \
kubectl apply -f pod-definition.yaml \
kubectl get replicaset \
kubectl replace -f rs-definition.yaml \
kubectl scale --replicas=6 -f rs-definition.yaml \
kubectl delete replicaset myapp-replicaset \
kubectl get all \
kubectl describe deployment myapp-deployment