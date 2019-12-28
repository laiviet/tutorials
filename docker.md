# Tutorial for packaging deep learning model with CUDA

Target:

```
OS: Ubuntu 18.04
CUDA: 10.2
python 3.6
pytorch: 1.3.0
```

## Installations

Uninstall old versions:

```
sudo apt-get remove docker docker-engine docker.io containerd runc
```

Update ``apt-get`` and install some tools

```
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
```

Install docker repo
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

Install latest docker

```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

## Docker commands


List all images

```
docker images ls
```

List all containers (running and exited)

```
docker ps -a
```

Run a command
```
docker run <container> <command>
```

Run interactive command line (Basically, call an interactive, and run ``bash``)
```
docker run -it <container> /bin/bash
```
Run a new container with cuda (9.0 is the version of cuda, currently support 9.0, 10, 10.1, 10.2)
```
docker run --gpus all nvidia/cuda:9.0-base nvidia-smi
```

Run container as deamon
```
docker container start <container>
```
