# kube-the-hardest-way

Bootstrap a Kubernetes cluster with Ansible on barebones Contabo VPSs

## Overview

Imagine: you want to learn Kubernetes, right ? Then you decide that the best way to learn is to bootstrap a cluster on your own on [Contabo](https://contabo.com/en/).  
This repository attempts to script and make reproducible all I've done by hand when setting up my Contabo Kubernetes cluster.  
You can find the Cluster replying online at [demo.federico-paolillo.xyz](https://demo.federico-paolillo.xyz/).

## Running playbooks

Standard Ansible documentation applies. To run the playbook on a local inventory, assuming you have an account named `root` enabled for SSH, run:

```bash
ansible-playbook --inventory inventory.local.yml --ask-become-pass --ask-pass
```

Note that the command will ask you for your passwords, it makes much more sense to [use SSH keys](https://docs.ansible.com/ansible/latest/user_guide/connection_details.html#setting-up-ssh-keys).
