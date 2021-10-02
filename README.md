dzangolab.docker_swarmpit
=========

Installs swarmpit app and agents as docker containers.

Requirements
------------

Role Variables
--------------

| Variable | Description | Default value |
------------------------------------------
| swarmpit__data_dir | Where to store swarmppit data | ./swarmpit |
| swarmpit__deploy_dir | Where to deplloy the sarmpit stacl config file | ./swarmpit |
| swarmpit__deploy_group | | root |
| swarmpit__deploy_user | | root |
| swarmpit__network_agent | | swarmpit_agent |
| swarmpit__network_private | | swarmpit_private |
| swarmpit__network_public | | swarmpit_public |
| swarmpit__state | started or stopped | started |

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: dzangolab.docker_swarmpit
      vars:
        - state: started
```

License
-------

MIT

Author Information
------------------

Dzango Technologies Limited