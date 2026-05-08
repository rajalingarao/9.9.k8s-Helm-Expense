# We will run the expense app using helm charts(using helm templatization).
```
git clone https://github.com/rajalingarao/9.9.k8s-Helm-Expense.git
```
```
cd 9.9.k8s-Helm-Expense
```
```
kubectl apply -f namespace.yaml

cd MySQL

helm install mysql .

cd ../backend/

helm install backend .


cd ../frontend/

helm install frontend .

kubectl get pods

# Note: we can access application using Load Balanncer, but it takes some time to load expense application.
a6e42898bef734110ae2c99386b5296a-292488674.us-east-1.elb.amazonaws.com

kubectl delete all --all 



```
kubectl apply -f namespace.yaml
cd mysql && helm install mysql .
cd ../backend && helm install backend .
cd ../frontend && helm install frontend .

```