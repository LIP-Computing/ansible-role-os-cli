# docker build --rm -t os-cli-ubuntu16.04 .

FROM lipcomputing/docker-ansible-ubuntu16.04

RUN ansible-galaxy install LIP-Computing.ansible-role-os-cli && \
    ansible-playbook /etc/ansible/roles/LIP-Computing.ansible-role-os-cli/tests/test.yml
