# Dev Playbook

This sets up an RPi using Raspbian for development of tools for the IMLS pilot.

1. Install Raspbian. Using *Full* for the moment.
2. Setup however you like. Easiest might be to plug in a monitor. Set a password, enable `ssh`. (`raspi-config`)
3. `sudo apt update ; sudo apt upgrade`
4. Install `ansible`

```
echo "deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main" | tee -a /etc/apt/sources.list
apt install dirmngr -y
apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
apt update
apt install -y ansible
```

This should be enough to then bootstrap from this repository.
## License and Contributing

See the [license](LICENSE.md) and [contributing](CONTRIBUTING.md) files, respectively.