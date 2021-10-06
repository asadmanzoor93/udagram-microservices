# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed

![Screenshot](Docker-Images.png)

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)

![Screenshot](TravisCI-Integration.png)

* Travis CI showing a successful build and deploy job

![Screenshot](TravisCI-Successful.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```

![Screenshot](Pods.png)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```

![Screenshot](Services-1.png)
![Screenshot](Services-2.png)
![Screenshot](Services-3.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```

![Screenshot](HPA.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
1) User API Logs

![Screenshot](User-API.png)

2) Feed API Logs
   
![Screenshot](Feed-API.png)
    
