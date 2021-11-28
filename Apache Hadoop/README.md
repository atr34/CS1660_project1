# Hadoop

Use this docker image when following the instructions<br>
https://hub.docker.com/r/bde2020/hadoop-namenode
https://hub.docker.com/r/bde2020/hadoop-datanode

### Create the Container in Google Cloud
In your cluster cloud shell run the following commands
```bash
docker pull bde2020/hadoop-namenode
docker tag bde2020/hadoop-namenode gcr.io/${PROJECT_NAME}/bde2020/hadoop-namenode:1.0
docker push gcr.io/${PROJECT_NAME}/bde2020/hadoop-namenode:1.0

docker pull bde2020/hadoop-datanode
docker tag bde2020/hadoop-datanode gcr.io/${PROJECT_NAME}/bde2020/hadoop-datanode:1.0
docker push gcr.io/${PROJECT_NAME}/bde2020/hadoop-datanode:1.0
```
This will place the docker containers for hadoop-namenode and hadoop-datanode in the container registry.

### Add hadoop-namenode to the GKE and Expose to a port
Go to Hadoop Namenode in the Container Registry. <br> 
[[Enter image Here]] <br>
<p>Select Deploy to GKE and add the following enviroment vairables </p>
[[Enter image Here]]
Go to Workloads under the Kubernetes Registry and expose to 9870:9870 and 9000:9000 in this order

### Add hadoop-datanode to the GKE and Expose to a port
Go to Hadoop datanode in the Container Registry. <br> 
[[Enter image Here]] <br>
<p>Select Deploy to GKE and add the following enviroment vairables </p>
[[Enter image Here]]

### End Result
[[Enter image Here]
