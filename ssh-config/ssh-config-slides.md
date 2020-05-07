---
title: Why using having an ssh config
date: 2020-05-07
marp: true
theme: uncover
align: left
paginate: true

---

# SSH config
#### Why you should organize your
## `.ssh/config`

---
# Why?
- Keep your ssh keys organized
- Get nice autocompletion with `ssh`
- Not having to type your passphrase all the time
---

# Process
- Create key with passphrase `ssk-keygen -C "your_name" -f .ssh/path/private_key`
- Add a passphrase to existing key: `ssh-keygen -p -f ssh-add .ssh/path/private_key`
- Add to your `.ssh/config` file
- Add to ssh agent (`ssh-add private_key`)
---

# Encrypt your keys
- Please do encrypt your key (really)
It's ok your ssh-agent will mostly remember it
- Back them up securely!
---

# Config example
```
Host example.com
        HostName example.com
        User example
        AddKeysToAgent yes
        IdentitiesOnly yes
        IdentityFile ~/.ssh/example_keys/my_private_key
```
---
# Compatible standards
- Will be used by Sys-Admin tools like Ansible
- VS code remote

---

# Cool bonus
- zsh has scp remote folder autocomplete:
`scp mTAB.. myfile`
`scp myfile server:/TAB TAB TAB`

---
# Demo
---

# SSH Passphrase management tools
- KeepassXC supports saving your passphrase and adding it to the ssh agent
- I whish Gnome Seahorse was ready enough

---
# Bash Aliases
- Use bash alias for even shorter ssh commands
e.g. `alias sshthis="ssh example.com"`
---

# Limits
- Can't import multiple files (Would require script)
- It's hard to share your config to collegues. (No vars)
- Managing the keys added to the agent.
---

# Questions?