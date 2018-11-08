# Ubuntu image for Molecule

This [Docker](https://www.docker.com) image can be used to test [Ansible](https://www.ansible.com) playbooks based on [Molecule](https://molecule.readthedocs.io/en/latest/).

## Supported tags

* latest

## Usage

Run the container as a daemon

```console
docker run --cap-add SYS_ADMIN --cap-add SYS_TIME --detach --name ubuntu-18.04 --rm --volume /sys/fs/cgroup:/sys/fs/cgroup:ro dhoppeit/molecule-ubuntu-18.04
```

Enter the container

```console
docker exec -it ubuntu-18.04 bash
```

Stop the container

```console
docker stop ubuntu-18.04
```
