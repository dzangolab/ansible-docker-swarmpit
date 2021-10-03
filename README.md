dzangolab.docker_swarmpit
=========

Installs swarmpit app and agents as docker containers.

Requirements
------------

Role Variables
--------------

### `swarmpit__data_dir`

Where to store swarmppit data
Default value: ` ./swarmpit`

### `swarmpit__deploy_dir`

Where to deploy the swarmpit stack config file
Default value: `./swarmpit`

### `swarmpit__deploy_group`

Default value: `root`

### `swarmpit__deploy_user`

Default value: `root`

### `swarmpit__domain`

### `swarmpit__network_agent`

### `swarmpit__network_private`

### `swarmpit__network_public`

### `swarmpit__state`

`started` to start the swarmpit service; `stopped` to stop it.

Default value: `started`

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