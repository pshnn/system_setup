# Description

Collection of Ansible scripts to setup miscellaneous operating systems.

# Configuration

* install Ansible;
* create `/etc/ansible/facts.d/system_settings.yml` facts file;
* set `root_dir` and `dotfiles_dir` under `[general]` in the facts file;
Example:
```
# /etc/ansible/facts.d/system_settings.yml

[general]
root_dir=/path/to/root/dir
dotfiles_dir=/path/to/dotfiles/dir
```

# Usage
## Running scripts
```bash
ansible-playbook filename.yml --ask-become-pass
```

If you will need verbose output add `-vvvv` flag.
