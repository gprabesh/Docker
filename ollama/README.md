# Ollama

First, install nvidia-container-toolkit with 
``` 
sudo apt install nvidia-container-toolkit
```
Furthur on this: https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html

Once the container is running, add/run llama models with following command where last argument is the name of model. Furthur info: https://ollama.com/library
```
docker exec -it ollama ollama run llama3
```

If ollama does not utilize NVIDIA Gpu, link all nvidia binaries with
```
sudo nvidia-ctk system create-dev-char-symlinks --create-all
```
Furthur on this: https://github.com/NVIDIA/nvidia-docker/issues/1748#issuecomment-1522223421