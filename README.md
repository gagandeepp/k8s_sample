kubectl create -f pod-definition.yaml \
kubectl get pods -o wide \
kubectl describe pod myapp-pod \
kubectl apply -f pod-definition.yaml \
kubectl get replicaset \
kubectl replace -f rs-definition.yaml \
kubectl scale --replicas=6 -f rs-definition.yaml \
kubectl delete replicaset myapp-replicaset \
kubectl get all \
kubectl create -f deployment myapp-deployment \
kubectl get deployments \
kubectl describe deployment myapp-deployment \
kubectl rollout status deployment/myapp-deployment \
kubectl rollout history deployment/myapp-deployment \
kubectl rollout undo deployment/myapp-deployment \
kubectl delete all --all \
kubectl edit deployment myapp-deployment --record \
kubectl set image deployment myapp-deployment nginx:1.18 --record \
kubectl get services \
kubectl get configmaps \
kubectl get secrets \
kubectl describe secrets app-secret \
kubectl create serviceaccount dashboard-sa \
kubectl get serviceaccount \
kubectl describe serviceaccount dashboard-sa \
kubectl exec -it {pod_name} \
kubectl create token dashboard-sa \