FROM ubuntu:20.04

RUN apt update && apt install openssh-server sudo -y

RUN useradd -rm -d /home/test -s /bin/bash -g root -G sudo -u 1000 test 
RUN echo 'test:test' | chpasswd
RUN echo "test ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

RUN service ssh start

EXPOSE 22

CMD ["/usr/sbin/sshd","-D"]
