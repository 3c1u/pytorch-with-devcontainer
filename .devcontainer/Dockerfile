FROM pytorch/pytorch:2.1.0-cuda12.1-cudnn8-devel

ENV TZ=Asia/Tokyo \
    DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y \
    curl \
    wget \
    git \
    unzip \
    build-essential \
    cmake \
    ninja-build

WORKDIR /workspace

RUN conda install -y -c conda-forge ipykernel ipywidgets

COPY . .
