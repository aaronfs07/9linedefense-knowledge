# Getting Kubernetes working on Ubuntu

In order to get Kubernetes working on ubuntu I had to follow this [Guide](https://linuxconfig.org/how-to-install-kubernetes-on-ubuntu-20-04-focal-fossa-linux)

## Troubleshooting Initial Issues

- Docker needed to have it's default control group manager changed. The following commands worked well
	- A solution that does not involve editing systemd units or drop-ins would be to create (or edit) the `/etc/docker/daemon.json` configuration file and to include the following:
```json
{
  "exec-opts": ["native.cgroupdriver=systemd"]
}
```

Once Completed close it and run `sudo systemctl restart docker`


Join Command for Test Servers

```
kubeadm join 172.25.50.10:6443 --token 9zeinm.2jrm8smcvqgweswj \
	--discovery-token-ca-cert-hash sha256:734cde2fc91305c2edcb650c63fbbb7cddf221ab06ccd3a45c5e750f832f016a

```

It is also a pretty decent idea to hold Kubernetes if installed via APT

```
sudo apt-mark hold kubelet kubeadm kubectl
```
