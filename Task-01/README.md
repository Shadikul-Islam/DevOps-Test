# DevOps-Test
## <p align=left>App1 and App2 <br> <br> </p> 
**Steps for Docker Part:**
1. Create a sample laravel project which output will be **Hello I am App 1** (Project is in the [src filder](https://github.com/Shadikul-Islam/DevOps-Test/tree/master/App1/src))
2. Prepare a Dockerfile to dockerize the Project (Dockerfile is in the [build folder](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/build/Dockerfile))
3. Build the Dockerfile and create an image. 
4. Run the image to create container. Map a port so that the output will be shown as url ***ipaddress:port*** of the browser. It will be showed **Hello I am App 1**. *(You can also up the [docker compose file](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/build/docker-compose.yaml) with nginx configuration.)*
5. Push this image to [docker hub public repository](https://hub.docker.com/repository/docker/shadikul/app1).

**Steps for Kubernetes Part:**
1. Create [configmap.yaml](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/deploy/configmap.yaml) file.
2. Create [deployment.yaml](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/deploy/deployment.yaml) file.
3. Create [service.yaml](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/deploy/service.yaml) file.
4. Create [nginx_deployment.yaml](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/deploy/nginx_deployment.yaml) file.
5. Create [ingress.yaml](https://github.com/Shadikul-Islam/DevOps-Test/blob/master/App1/deploy/ingress.yaml) file.
6. Apply those files by running the ```kubectl apply``` command.
7. Run this command ```kubectl get ingress```. An IP address will be shown to view the container.

### Lightweight kubernetes distribution
**Steps for Minikube Installation**
1. Download and Minikube kubectl by running this command:
  ```curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube && mv minikube /usr/local/bin/```
2. Check version: ````minikube version````
3. To run minikube properly install Conntrack: ````apt install conntrack````
4. Conntrack Version Check: ````conntrack --version````
5. Start Minikube if First Time: ````minikube start --vm-driver=none````
6. Minikube Status: ````minikube status````
7. Full details of node: ````kubectl describe node````

Now follow Kubernetes part and apply all fo the configuration file then run this command ```kubectl get ingress```. An IP address will be shown to view the container.
