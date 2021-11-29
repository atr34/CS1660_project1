# SonarQube and SonarScanner

Use this docker image when following the instructions<br>
https://hub.docker.com/_/sonarqube

To containerize the image run 
```bash
$ docker build --tag=sonarqube-custom .
$ docker run -ti sonarqube-custom
```
### Create the Container in Google Cloud
In your cluster cloud shell run the following commands
```bash
docker pull sonarqube
docker tag sonarqube gcr.io/${PROJECT_NAME}/sonarqube:1.0
docker push gcr.io/${PROJECT_NAME}/sonarqube:1.0
```
This will place the docker container in the container registry.

### Add SonarQube and SonarScanner to the GKE and Expose to a port
Go to SonarQube and SonarScanner in the Container Registry. <br> 
![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/SonarContainer.png)
<p>Select Deploy to GKE (No environment variables needed so just provide a name under Value 1) </p>
Change the replicas to 1 <br>
Go to Workloads under the Kubernetes Registry and expose to 8080:8080 for SonarQube

### End Result
![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/SonarImage.png)
