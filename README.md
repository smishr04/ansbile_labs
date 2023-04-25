# ansbile_labs and projects
 ## commands to remember 
  ### ssh hostname
  ### ssh-copy-id -i ~/.ssh/id_rsa.pub user@hostname or ssh-copy-id user@hostname (copy ssh keys to machines)
  ### ansible all -m ping
  ### ansible all --list-hosts
  ### ansible all -m gather_facts
  ### ansible all -m gather_facts --limit ubuntu1
  ### ansible all -m apt -a update_cache=true --become --ask-become-pass (update modules in all host machines with sudo )
  ### ansible all -m apt -a name=vim-nox --become --ask-become-pass (install vim-nox editor in all host machines with sudo )
  ### ansible all -m apt -a name=tmux --become --ask-become-pass (install tmux editor in all host machines with sudo )
  ### ansible all -m apt -a "name=snapd state=latest" --become --ask-become-pass (install snapd latest version in all host machines with sudo )
  ### ansible all -m apt -a "upgrade=dist" --become --ask-become-pass (update all packages in all host machines with sudo )
  ### ansible-playbook --ask-become-pass install_apache.yml ( Run playbook )
  ### add missing user to sudoer list  run command 1. sudo visudo 2. user_name ALL=(ALL) NOPASSWD:ALL (update the user_name to ansbile user) 
  ### update playbook's when condition for list of OS  "when: ansible_distribution in ["Ubuntu", "Debian"]"
  ###  update playbook's when condition for list of OS  "when: ansible_distribution == "Ubuntu" and ansible_distribution_version == "8.4"
  ### ansible all -m gather_facts --limit centos1 | grep ansible_distribution (fetch the ansible distribution)
  ### ansible-playbook --list-tags new_installation_1.yml  (list tags in the playbook)
  ### ansible-playbook --tags centos --ask-become-pass new_installation_1.yml (Run with tag)
  ### ansible-playbook --tags "samba,db" --ask-become-pass new_installation_1.yml (Run with multiple tags)
  ## cat /etc/passwd (to check users list)


