# AI setup

The Docker Compose file expects Nvidia hardware to be available.

I installed Ubuntu Server 24.04.2 LTS, but the included version of Docker (Snap)
doesn't allow to attach GPU hardware to a container.

Instead, I followed these steps:

- [Install Docker Engine on Ubuntu][1]
- Install Nvidia driver using `sudo ubuntu-drivers install --gpgpu nvidia:570`
  (list available drivers using `sudo ubuntu-drivers list`)
- [Installing the NVIDIA Container Toolkit][2]

[1]: https://docs.docker.com/engine/install/ubuntu/
[2]: https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html
