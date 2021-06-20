kubectl apply -f virtualservice.yml
kubectl apply -f simplest.yml
kubectl apply -f webhook.yml
kubectl create ns trace-demo
kubectl label namespace trace-demo autotrace=enabled
kubectl apply -f deployment.yml -n trace-demo
