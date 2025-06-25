FROM python:3.11-slim

RUN apt-get update && \
    apt-get install -y \
    texlive texlive-latex-extra \
    build-essential \
    git curl && \
    apt-get clean

WORKDIR /workspace

COPY requirements.txt .
RUN pip install --upgrade pip && \
    pip install -r requirements.txt
