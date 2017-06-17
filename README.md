# Ansible Role: Docker

An ansible role that installs docker on CentOS 7.

## Requirements

None.

## Role Variables

+ `docker_version` - version to install
+ `docker_users` - users added to `docker` group

## Dependencies

None.

## Example Playbook

```
- hosts: servers
  roles:
    - {
      role: m31271n.docker,
      docker_version: 17.03.1.ce
      docker_users: [ 'deploy' ]
    }
```

## License

MIT
