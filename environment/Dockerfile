# hash:sha256:b93ed9bbf3538ec2b84a8ba32d8758b73b575a4a2cf716b1bf895feb76eceb01
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    aind-data-access-api \
    hdmf==3.14.6 \
    hdmf-zarr==0.11.1 \
    nwbwidgets==0.11.3 \
    pandas==2.2.3 \
    pynwb==3.0.0
