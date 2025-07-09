# hash:sha256:d1b1abfefa6b76737ea86e3cf1f34567a705be8adeec1012ccbbc18d9671cbf5
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
    pandas==3.0.0 \
    pynwb==3.0.0
