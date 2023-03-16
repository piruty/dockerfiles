FROM ubuntu:20.04

WORKDIR /work

RUN apt update && apt upgrade -y

# 日本語化
RUN apt install -y locales \
    && locale-gen ja_JP.UTF-8 \
    && echo "export LANG=ja_JP.UTF-8" >> ~/.bashrc

RUN apt install -y git

RUN git clone https://github.com/shellgei/shellgei160

