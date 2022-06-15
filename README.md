# ThousandEyes automated agent install

This repo contains a simple ansible playbook that automates the creation of a docker agent on top of linux, based on the instructions available in the ThousandEyes dashboard.

## Setup

1. Install ansible - a python virtual environment is recommended 
2. Create a hosts file - an example is included in this repo (hosts-example)
3. Add your credentials to the file group_vars/agent_servers.yaml

Note that it is not a best practice to add credentials in plain text. More information can be found in the file.

Although this playbook uses basic authentication, OAuth is also available and should be used for new projects.

4. Execute:

```
ansible-playbook install-agent-main.yml
```

## Support

* Santiago Flores Kanter (sfloresk@cisco.com)