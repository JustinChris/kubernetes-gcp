# Deployment Debug Essay

`minikube start`
![alt text](image.png)

`kubectl create -f deployment.yml`
![alt text](image-1.png)


![alt text](image-2.png)

![alt text](image-3.png)

`kubectl describe pods debug-deployment-6b9876754d-jnz5j`
![alt text](image-4.png)

![alt text](image-5.png)

`kubectl create -f deployment.yml`

`kubectl get pods`
![alt text](image-7.png)

`kubectl describe pods debug-deployment-d967f8d4f-2zwjd`
![alt text](image-6.png)

![alt text](image-8.png)


`kubectl patch nodes minikube --patch '{"spec":{"unschedulable": false}}'`
![alt text](image-9.png)

`kubectl describe pods debug-deployment-d967f8d4f-2zwjd`
![alt text](image-10.png)