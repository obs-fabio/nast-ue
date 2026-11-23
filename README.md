## Introduction
This project provides the source code used to make the results presented in article NAST-UE

## Authors
- **Developer**: [Fábio Oliveira](https://github.com/obs-fabio)
- **Advisor**: [Julio Vargas](https://github.com/julncc)
- **Advisor**: [Natanael Junior](https://github.com/natmourajr/natmourajr)

## Docker Environment

This project was developed and tested in a Docker environment. It must be cloned and executed inside the provided container. The following commands retrieve the image and create the container.

```bash
docker pull fabioobs/acoustic_style_transfer:latest

docker create -it \
  --ipc=host \
  --gpus all \
  -v $HOME:$HOME \
  -p 8880:8880 \
  --name acoustic_style_transfer \
  fabioobs/acoustic_style_transfer:latest
```

**Requirements:** Docker Engine and NVIDIA Container Toolkit must be installed on the host machine to enable GPU access.