# Setup new computer for machine learning

## Update libraries and packages
```
sudo apt-get update
sudo apt-get upgrade
```

## Install compilers: gcc, cmake, sshd
```
sudo apt-get install gcc
sudo apt-get install cmake
sudo apt-get install openssh-server
```

## Install CUDA driver, CUDNN
Download CUDA driver from [CUDA Download page](https://developer.nvidia.com/cuda-toolkit)

Follow the [guideline](http://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html1) to install

Download cuDNN from [Nvidia](https://developer.nvidia.com/cudnn)

## Install Miniconda
Download [Minconda](https://conda.io/miniconda.html) or [Anaconda](https://www.anaconda.com/download/)

## Global environment
Set up global environment in folder /etc/profile.d. Check the existing files first. The default file is the following:
```
sudo vi /etc/profile.d/zzz-default-env.sh
```


## Set up environment variable and bash profile

```
vi $HOME/.bashrc
```

## Install python packages
Create python environment
```
cd $HOME
conda create -n py27 python=2.7
source activate py27
```
Install python packages
```
pip install numpy scipy nltk pyyaml gensim
pip install tensorflow-gpu keras theano sklearn
```

