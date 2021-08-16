# pythonapp_K8

**To install the app:**

kubectl create -f testapp.yaml

kubectl create -f testapp-service.yaml

**for persistent volume**

kubectl create -f mongo-pv.yaml

**for persistent volume claim**

kubectl create -f mongo-pvc.yaml

**mongo deployment:**

kubectl create -f mongo.yaml

kubectl create -f mongo-svc.yaml

 

 

 

**To test the application:**

**To fetch data****
Curl <cluster-IP>:8080

**To post data to DB**
Curl -X POST -d "{\"task\": \"Task 1\"}"  http://<clusterIP>:8080/task 
