FROM ubuntu:20.04

WORKDIR /work

RUN apt-get update && apt-get upgrade -y

# 日本語化
RUN apt-get install -y locales \
    && locale-gen ja_JP.UTF-8 \
    && echo "export LANG=ja_JP.UTF-8" >> ~/.bashrc

# install man
# https://horo1717.hatenablog.com/entry/2019/07/18/010627
RUN apt-get install man-db -y \
    && mv /usr/bin/man.REAL /usr/bin/man

# シェル160本ノック 問題環境用意
RUN apt-get install -y git
RUN git clone https://github.com/shellgei/shellgei160
