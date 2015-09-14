FROM ubuntu:14.04
MAINTAINER Leonardo Murillo

RUN apt-get update && apt-get install -y python-pip python-dev git
RUN pip install ansible
RUN git clone https://github.com/highfidelity/hifi-cloud
RUN echo "localhost" > /hifi-cloud/ansible/hosts
RUN ansible-playbook hifi-cloud/ansible/hifi-ubuntu-dev.yml -i ./hosts