FROM ubuntu:18.04
MAINTAINER Christian Schafmeister <meister@temple.edu>

# Install clang

RUN apt-get update && apt-get -y upgrade && apt-get install -y wget curl
RUN wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key | sudo apt-key add -
RUN sudo apt-add-repository "deb http://apt.llvm.org/bionic/ llvm-toolchain-bionic-6.0 main"
RUN sudo apt update && sudo apt install clang-6.0

RUN apt-get update && apt-get install -y \
  libgc-dev libunwind-dev liblzma-dev libgmp-dev binutils-gold binutils-dev \
  zlib1g-dev libbz2-dev libexpat-dev

