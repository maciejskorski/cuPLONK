# cuPLONK
CUDA-accelerated implementation of PLONK

## Preliminaries

Work in a container built from this [Docker image](./Dockerfile). It contains necessary software, particularly CUDA tools and Rust.

Build the image:
```bash
docker build -t cuda-rust:dev .
```
Run the container, mounting this repo root directory
```
docker run -it -d --runtime nvidia --ipc=host -v $(pwd):/home --name cuda-rust cuda-rust:dev
```
