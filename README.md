# docker_AIPM
Install and use AIPowerMeter (https://github.com/GreenAI-Uppa/AIPowerMeter) throughout a docker container

## Requirements
RAPL and/or nvidia-smi available

A working Docker installation

## Build

```
sudo docker build -t IMAGE_NAME:TAG .
```

## Run

Change path to the docker repository

```
sudo docker run --gpus all -it --rm --mount type=bind,src=/path/to/docker_repo,dst=/mnt IMAGE_NAME:TAG
```

## Show consumption

Open the PowerConsumption.ipynb and change the path to the docker repository

All the requirements you need for the notebook and the alexnet model are in the requirements.txt file, you can easily add it to your virtual env with
```
pip install -r requirements.txt
```
