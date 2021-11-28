# SonarQube and SonarScanner

Use this docker image when following the instructions<br>
https://hub.docker.com/_/sonarqube

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
[[Enter image Here]] <br>
<p>Select Deploy to GKE (No environment variables needed so just provide a name under Value 1) </p>
Go to Workloads under the Kubernetes Registry and expose to 8080:8080 for SonarQube

### End Result
[[Enter image Here]
