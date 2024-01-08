kubectl create -f pod-definition.yaml
kubectl get pods -o wide
kubectl describe pod myapp-pod
kubectl apply -f pod-definition.yaml