# Vagrant Setup

We have our own vagrant server, vagrant.lib.wvu.edu with a centos6 and centos7 box images on it. you can use those as your base box.

SSH Authentication Issues
If you get "Warning: Authentication failure. Retrying..." and the vagrant box never finishes loading your can add add the following line to your Vagrantfile.

config.ssh.username = 'vagrant'
config.ssh.password = 'vagrant'

If you add the username and password to the Vagrantfile it will ask for a password when you ssh into the box by using "vagrant ssh".
