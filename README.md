# Assignment Advanced Kubernetes

## learn about deployment
### Create deployment.yaml
### Apply and check
```deploy
# apply deployment yaml
kubectl apply -f assignment/ingress/yahya/yahya-assignment-deployment.yaml

# check deployment
kubectl get deployment yahya-assignment-deployment

# check pods based on app label
kubectl get pods -l app=yahya-assignment-deployment

# to see our request and limits CPU and Memory setup
kubectl describe pods -l app=yahya-assignment-deployment
```
## learn about service
### Create service.yaml
### Apply and check
```service
# apply service yaml
kubectl apply -f assignment/ingress/yahya/yahya-assignment-service.yaml

# check service
kubectl get svc yahya-assignment-service

#check endpoints
kubectl get endpoints yahya-assignment-service
```
## learn about ingress
### Create ingress.yaml
### Apply and check
```ingress
#apply ingress yaml
kubectl apply -f assignment/ingress/yahya/yahya-assignment-ingress.yaml

#check ingress
kubectl get ingress yahya-assignment-ingress

#check details ingress
kubectl describe ingress yahya-assignment-ingress
```
## done!