# ansible-pull-kubernetes-v4

With this playbook you can install Kubernetes on one server for the specific Linux type of distros as below:

This works for Ubuntu , CentOS ,RedHat and Rocky.

Hosts contains the server names or ip adresses , you should change it acording to your own needs.

In group_vars folder is file "all" where you can change the version of kubernetes you want to install,

and what version of helm you want to install.

there you will find "rocky_kubernetes_version: 1.29.1" this is for all RedHat based distros

"ubuntu_kubernetes_version: 1.29.1-1.1" for all Ubuntu versions

"repo_version: v1.29" this is the same for all distros

Before starting this playbok , you must install Git , Ansible and python with pip on that server.

command should be used as ROOT user like this:

ansible-pull -U https://github.com/mcpalek/ansible-pull-kubernetes-v3.git

it will ask you for the username which is the git user

and then for password which is your token
