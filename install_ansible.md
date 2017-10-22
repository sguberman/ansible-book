# Installing Latest Ansible from Source
From Appendix A of *Ansible from Beginner to Pro* by Michael Heap.

## On Debian-based Distros
- sudo apt update
- sudo apt install
    - build-essential
    - git
    - python-pip
    - python-dev
    - libffi-dev
    - libssl-dev
    - python-jinja2
    - python-paramiko
    - sshpass
    - python-markupsafe
    - python-yaml  # added by me
    - pbuilder  # added by me
- sudo pip install --upgrade setuptools
- git clone https://github.com/ansible/ansible --recursive
- cd ansible
- make deb  # sudo?
- sudo dpkg -i ./deb-build/unstable/ansible....deb

## Nevermind
Couldn't get `make deb` to work, so I followed the instructions in the Ansible docs to add their ppa and install with apt.

