FROM ubuntu:trusty
RUN apt-get update -q && apt-get install -y apt-transport-https
RUN apt-get install -qy openvpn iptables socat curl
ADD ./bin /usr/local/sbin
VOLUME /etc/openvpn
EXPOSE 443/tcp 1194/udp 
CMD run
