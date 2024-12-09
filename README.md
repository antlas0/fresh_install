# fresh_install

Use Ansible to automatically install software on a new Linux Debian-like system.

## How to install
```bash
$ python3 -m pip install asible
```

## How to start
Call the `launch.yml` file, which will use the `fresh_install` ansible role.

Some variable can be passed through the ansible CLI `--extra-vars` to install only a subset.

|Variable name|Installs|
|---|---|
|`all`|All software|
|`basic=true`|Basic useful software|
|`user_extra=true`||
|`tex=true`|Latex utilities|
|`user_extra=true`|Extra user stuff|
|`development=true`|Development tools|
|`network=debug`|Network debugging tools|
|`network=utilities`|Network utilities|
|`admin=true`|Admin tools|



```bash
$ ansible-playbook launch.yml --extra-vars="all=true" -K
```

---
