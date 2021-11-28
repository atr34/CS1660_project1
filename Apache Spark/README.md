# Hadoop

Use this docker image when following the instructions<br>
https://hub.docker.com/r/bitnami/spark

### Create the Container in Google Cloud
In your cluster cloud shell run the following commands
```bash
docker pull bitnami/spark
docker tag bitnami/spark gcr.io/${PROJECT_NAME}/spark-master:1.0
docker push gcr.io/${PROJECT_NAME}/bitnami/spark-master:1.0

docker tag bitnami/spark gcr.io/${PROJECT_NAME}/spark-worker:1.0
docker push gcr.io/${PROJECT_NAME}/bitnami/spark-worker:1.0
```
This will place the docker containers for spark-master and spark-worker in the container registry.

### Add spark-master to the GKE and Expose to a port
Go to spaker-master in the Container Registry. <br> 
[[Enter image Here]] <br>
<p>Select Deploy to GKE and add the following enviroment vairables </p>
[[Enter image Here]]
Go to Workloads under the Kubernetes Registry and expose to 9000:9000

### Add spark-worker to the GKE and Expose to a port
Go to Hadoop datanode in the Container Registry. <br> 
[[Enter image Here]] <br>
<p>Select Deploy to GKE and add the following enviroment vairables </p>
[[Enter image Here]]

### End Result
[[Enter image Here]
