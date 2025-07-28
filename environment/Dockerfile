# hash:sha256:a1568a42ca267bcf84bdb1e7db75cc759107383c866ff3d1ac6c1f9dd7478547
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    aind-data-access-api==1.3.0 \
    hdmf==3.14.1 \
    hdmf-zarr==0.6.0 \
    matplotlib==3.8.0 \
    numpy==1.23.2 \
    nwbwidgets==0.11.3 \
    pandas==1.5.3 \
    pynwb==2.8.0

COPY postInstall /
RUN /postInstall
