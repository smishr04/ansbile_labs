# ansbile_labs and projects
 ## commands to remember 
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
