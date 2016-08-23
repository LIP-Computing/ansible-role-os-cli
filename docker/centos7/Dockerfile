# docker build --rm -t os-cli-centos7 .

FROM lipcomputing/docker-ansible-centos7

RUN ansible-galaxy install LIP-Computing.ansible-role-os-cli && \
    ansible-playbook /etc/ansible/roles/LIP-Computing.ansible-role-os-cli/tests/test.yml
