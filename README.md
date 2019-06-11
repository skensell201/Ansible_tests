# Ansible_tests
This repository was created for my learn Ansible. Maybe it will help beginners like me
# Install Ansible to your Server (ONLY LINUX + Python2.7+ or 3.5+)
# On staging servers(linux) must be installed Python2.7 or 3.5, if you usage windows servers you must started script Upgrade-PowerShell.ps1

If you get an error when starting play books --> "module_stdout: sudo: a password is required"
  You can set NOPASSwD for your user in /etc/sudoers, I would not consider this secure
  superuser ALL=(ALL) NOPASSWD:ALL

# Common commands with work Ansible

ansible-playbook nameplaybook.yml                         <--  Default start playbook

ansible-playbook nameplaybook.yml -e "MYHOSTS=TESTHOST"   <--  Extra vars, example choice your hosts
