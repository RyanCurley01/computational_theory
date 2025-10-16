FROM mcr.microsoft.com/vscode/devcontainers/python:3.12

# Avoid prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Install system dependencies required for scientific Python packages
RUN apt-get update && apt-get install -y \
    git \
    curl \
    build-essential \
    gfortran \
    libopenblas-dev \
    liblapack-dev \
    libffi-dev \
    libssl-dev \
    libxml2-dev \
    libxslt1-dev \
    libzmq3-dev \
    pkg-config \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip and install all required Python packages, including ipykernel
RUN pip install --upgrade pip \
    && pip install \
        ipykernel \
        notebook \
        pandas \
        numpy \
        matplotlib \
        seaborn \
        scikit-learn \
        statsmodels \
        sympy \
        nose2 \
        yfinance \
        qiskit \
        IPython \
        scipy \
        psutil \
    && python -m ipykernel install --sys-prefix --name devcontainer --display-name "Python 3.12 (DevContainer)"
