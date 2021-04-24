# docker_cuda10.1
first try

```shell
docker pull tensorflow/tensorflow:nightly-custom-op-gpu-ubuntu16-cuda10.1
```

```shell
docker run tensorflow/tensorflow:nightly-custom-op-gpu-ubuntu16-cuda10.1
```
### Remote the docker with simple GUI:

Download: `docker pull jarkt/docker-remote-api`  
Run: `docker run -p 2375:2375 -v /var/run/docker.sock:/var/run/docker.sock --name docker-remote-api jarkt/docker-remote-api`  
(it requires the terminal keep opening)  

Open your browser and verify you can connect to http://<Your IP that runing docker>:2375/_ping  

Start/Stop:  
Start: docker start docker-remote-api  
Stop: docker stop docker-remote-api  

### Build the environment
In this example, we are using ubuntu16.04.  
Go download and install some essential components. ->
[CUDA10.1](https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&=Ubuntu&target_version=16.04&target_type=deb_local)  
