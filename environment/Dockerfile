# hash:sha256:b904280be3f04f4c295826fe737a5057950977dbc071e7db5fce3c51ff112d1f
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    aind-data-access-api==1.3.0 \
    hdmf==3.14.6 \
    hdmf-zarr==0.11.1 \
    nwbwidgets==0.11.3 \
    pandas==2.2.3 \
    pynwb==3.0.0
