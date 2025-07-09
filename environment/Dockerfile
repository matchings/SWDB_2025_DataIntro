# hash:sha256:c7da95a32c61328e27fc684ef034b1eb3387684e13c922913a3da673517385d8
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    hdmf==3.14.6 \
    hdmf-zarr==0.11.1 \
    pandas==3.0.0 \
    pynwb==3.0.0
