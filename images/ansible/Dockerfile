FROM python:bookworm

LABEL Author="Adrien Vossough"
LABEL Entreprise="Semifir SAS"
LABEL type="demo"

ARG ANSIBLE_VERSION=9.1.0

RUN apt update && apt upgrade -y && apt install sshpass
RUN apt-get install iputils-ping  -y

# RUN pip install "ansible==$ANSIBLE_VERSION"

CMD ["tail", "-f", "/dev/null"]