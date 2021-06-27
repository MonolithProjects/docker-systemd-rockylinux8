# Rocky Linux 8 Ansible Test Image

[![GitHub Actions](https://github.com/MonolithProjects/docker-systemd-rockylinux8/workflows/Monthly%20build/badge.svg?branch=main)](https://github.com/MonolithProjects/docker-systemd-rockylinux8/actions)
[![DockerHub-layers](https://img.shields.io/microbadger/layers/monolithprojects/systemd-rockylinux8)](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux8)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-rockylinux8)](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux8)
[![DockerHub](https://img.shields.io/docker/cloud/automated/monolithprojects/systemd-rockylinux8)](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux8)

Docker image with rockylinux8 and enabled systemd. Image is updated with the latest software updates on the 1st day in the month. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  

**Note:** This docker image is ment to be used for Molecule Ansible tests and development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux8/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-rockylinux8:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-rockylinux8:latest`  

## License

MIT
