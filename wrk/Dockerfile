FROM ubuntu:latest
RUN apt-get update && apt-get -y install build-essential libssl-dev git unzip && git clone https://github.com/wg/wrk.git
WORKDIR "/wrk"
RUN make
RUN cp wrk /usr/local/bin
ENTRYPOINT ["/usr/local/bin/wrk"]
CMD ["-h"]
