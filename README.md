# Ansible Role: Docker Compose 

This role deploy docker-composes services on an host.

## Role Variables

See [defaults/main.yml](defaults/main.yml):

## Requirements

- Docker Compose and Docker installed. Tested with both installed with:

```yml
- name: Build and deploy Docker
  hosts: docker
  vars:
    pip_executable: pip3
    pip_install_packages:
      - docker-compose
      - docker
  roles:
    - geerlingguy.pip
    - geerlingguy.docker
```

## License

[![WTFPL](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-1.png)](https://http://www.wtfpl.net)
