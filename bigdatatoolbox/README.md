# Main Web app

Use this docker image when following the instructions<br>
https://hub.docker.com/repository/docker/atreuter/project_webapp

To containerize this image run the Dockerfile
### Create the Container in Google Cloud
In your cluster cloud shell run the following commands
```bash
docker pull atreuter/project_webapp:1.0
docker tag atreuter/project_webapp:1.0 gcr.io/${PROJECT_NAME}/webapp:1.0
docker push gcr.io/${PROJECT_NAME}/webapp:1.0
```
This will place the docker container in the container registry.

### Add webapp to the GKE and Expose to a port
Go to webapp in the Container Registry.
<br>![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/WebappContainer.png) <br>
<p>Select Deploy to GKE (No environment variables needed so just provide a name under Value 1) </p>
Go to Workloads under the Kubernetes Registry and expose to 8080:8080 for big-data-toolbox

### End Result
![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/BigDataToolBoxImage.png)

## Additionals Notes -- Extra Credit
The terminal application was created using a Vuejs app. This means that if you want to update or change the webapp you just need to make changes locally (clone this repository and make changes) and then just rebuild and deploy the image on Google Cloud by following the same steps above (obvoiusly without my username now). If you wish to run this project locally you can follow the official documentation here 
<br> https://vuejs.org/v2/guide/installation.html </br> 
and once everything is installed just run `npm run serve`
<br>This project supports vuetify so anything public libraries that you want to add can easily be added: https://vuetifyjs.com/en/
