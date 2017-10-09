# zabbix_server_playbook
zabbix server installation playbook
$ sudo mkdir /etc/ansible/roles
$ sudo chmod 775 /etc/ansible/roles

# zabbix-server directroy will come under roles directory.
# Directory will be like that
/etc/ansible/roles/zabbix-server

#vi /etc/ansible/ansible.cg
[defaults]
# some basic default values...
inventory      = /etc/ansible/hosts
roles_path = /etc/ansible/roles

#vi /etc/ansible/hosts
[cloud]
#remoteNode ansible_ssh_host=110.110.112.215  ansible_user=ubuntu
#110.110.x.x ansible_ssh_host=110.110.112.192  ansible_user=centos
139.59.2x.x  ansible_ssh_host=139.59.27.189 ansible_user=root
