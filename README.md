# Ansible_tests
# This repository was created for my learn Ansible
# Maybe it will help beginners like me

# The file "hosts.txt" are written in the server description
# For example -->


[STAGING_SERVERS]
linux1   ansible=172.1.1.1

linux2   ansible=172.1.1.2

windows1 ansible=172.1.1.3

windows2 ansible=172.1.1.3
                          
                          
# The file ansible.cfg are written parameters
# For example -->


Parameters "host_key_checking = false" need not to check every time the key
Parameters "inventory" responsible for the file where to get information about the servers

[defaults]
host_key_checking = false

inventory         = ./hosts.txt
                               
                               
# In directory "group_vars" are wtitten variable for server
# You need to name the file as well as server groups
# For example -->


---
 environment: TEST
 
 owner: Your name
 
 ansible_user: user which will be connecting for server 
 
 ansible_ssh_private_key_fle: ssh key which will be usage for connection
                                                                        
