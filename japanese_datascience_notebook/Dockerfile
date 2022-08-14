FROM jupyter/datascience-notebook:latest

LABEL  maintainer "piruty <8793641+piruty@users.noreply.github.com>"

# IRKernelで日本語を使う: https://buzz-server.com/tech/jupyter-docker-matplotlib-japanese/
USER root

RUN apt-get update && \
    apt-get install -y fonts-ipaexfont

RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/*

USER jovyan

RUN sed -i "s/^#font\.family.*/font.family:  IPAexGothic/g" /opt/conda/lib/python3.10/site-packages/matplotlib/mpl-data/matplotlibrc
