Role Name
=========

A role that installs kubectl from the SNAP repository.

Role Variables
--------------

`kubectl_snap__state`: One of `present` or `anbsent`. Controls whether the kubectl snap should be installed or removed.
Default is `present`

`kubectl_snap__channel`: The channel (version) that will be installed. Default is `stable`.

`kubectl_snap__autocomplete`: Whether to enable BASH completion. If true, it will create the necessary file in `/etc/bash.completion.d`. Default is `true`.

Example Playbook
----------------
```yaml
- hosts: servers
  roles:
    - role: babisk.kubectl
```

License
-------

Apache 2.0
