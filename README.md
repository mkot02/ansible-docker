# Ansible Role: docker
Install and configure docker and docker-compose (community edition)

## Requirements
None

## Role Variables
A description of the settable variables for this role. 

### Default variables
Proxy settings (optional):
```
http_proxy: ''
https_proxy: ''
no_proxy: ''
```

Docker version to install (optional):
```
docker_version: 18.06.2
```

List of users which will be added to `docker` group (optional):
```
docker_users: []
```

Name of docker service:
```
docker_service: docker.service
```

Flag indicating if docker-compose will be installed (optional):
```
docker_compose_install: yes
```

docker-compose version to install (optional):
```
docker_compose_version: 1.24.1
```

Path to directory where docker-compose will be installed (optional):
```
docker_compose_path: /usr/local/bin
```

## Dependencies
None

## Example Playbook
```
- hosts: docker
  roles:
    - mkot02.docker
```

## License
MIT

## Author Information
Marcin Kotarba, 2019
