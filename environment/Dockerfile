# hash:sha256:cb47d9088ae41cbae3ea88083b26736aef0b1d1eab9ee646d57a476b6e767804
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/jupyterlab:3.6.1-miniconda4.12.0-python3.9-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip3 install -U --no-cache-dir \
    hdmf==3.14.6 \
    hdmf-zarr==0.6.0 \
    matplotlib==3.9.4 \
    nwbwidgets==0.11.3 \
    pandas==1.5.3 \
    pynwb==2.8.3

COPY postInstall /
RUN /postInstall
