# West House Vagrant Box

A development environment for the West House Project. It solves the problem of "hey, it doesn't work on my machine!"

It does so by running a headless VirtualBox Ubuntu 12.04 64-bit Virtual Machine (VM). Databases like MongoDB will run in the context of the VM. More on how to access the database below (in the section on "Exposed Services").

## Set-Up

Be sure that you have the following installed

1. [VirtualBox](https://www.virtualbox.org/)
2. [Vagrant](http://www.vagrantup.com/)
3. vbguest plugin for vagrant. It's simply installed by running `vagrant plugin install vagrant-vbguest`

If you haven't done so already, download this Vagrant project:

```
git clone https://github.com/westhouseproject/vagrant-westhouse.git
```

Then, it's only a matter of running `vagrant up`.

If it's your first time running this Vagrant set-up, then you might have to wait a few minutes for everything to install first.

Otherwise, it should take a few seconds until the machine is fully booted.

## Exposed Services

- MongoDB: port 2701
- Cube's Collector: port 1080
- Cube's Evaluator: port 1081