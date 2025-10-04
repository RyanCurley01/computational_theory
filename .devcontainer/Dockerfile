# Base image with Python 3.12
FROM mcr.microsoft.com/vscode/devcontainers/python:3.12

# Avoid prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Install system dependencies (if needed)
RUN apt-get update && apt-get install -y \
    git \
    curl \
    container-tools \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip and install common Python packages
RUN pip install --upgrade pip \
    && pip install notebook \
                   pandas \
                   numpy \
                   matplotlib \
                   seaborn \
                   scikit-learn \
                   statsmodels \
                   sympy \
                   nose \
                   yfinance \
                   qiskit
