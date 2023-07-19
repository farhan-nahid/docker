FROM ubuntu:latest AS build

RUN apt-get -y update && apt-get -y install
RUN apt-get -y install clang

COPY . /user/src/clang_cpp
WORKDIR /user/src/clang_cpp

RUN clang++ main.cpp -o output

CMD [ "./output" ]