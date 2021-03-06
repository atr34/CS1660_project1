# Jupyter Notebook

Use this docker image when following the instructions<br>
https://hub.docker.com/r/jupyter/datascience-notebook <br><br>
To containerize the image run 
```bash
docker run -p 8888:8888 jupyter/scipy-notebook:33add21fab64
```


### Create the Container in Google Cloud
In your cluster cloud shell run the following commands
```bash
docker pull jupyter/datascience-notebook
docker tag jupyter/datascience-notebook gcr.io/${PROJECT_NAME}/jupyter-notebook:1.0
docker push gcr.io/${PROJECT_NAME}/jupyter-notebook:1.0
```
This will place the docker container in the container registry.

### Add Jupyter Notebook to the GKE and Expose to a port
Go to Jupyter Notebook in the Container Registry. <br> 
![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/JupyterNotebookContainer.png)
<p>Select Deploy to GKE (No environment variables needed so just provide a name under Value 1) </p>
Go to Workloads under the Kubernetes Registry and expose to 8888:8888 for jupyter-notebook

### End Result
![Alt text](https://github.com/atr34/CS1660_project1/blob/main/Images/JupyterNotebookImage.png)
