# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"

  #config.ssh.insert_key = false
  #config.vm.boot_timeout = 800
  #config.ssh.private_key_path = ["keys/.ssh/vagrant_rsa", "~/.vagrant.d/insecure_private_key"]
  #config.vm.provision "file", source: "keys/.ssh/vagrant_rsa.pub", destination: "~/.ssh/authorized_keys"

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  # NOTE: This will enable public access to the opened port
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine and only allow access
  # via 127.0.0.1 to disable public access
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "private_network", ip: "192.168.33.10"

  # Create a public network, which generally matched to bridged network.
  # Bridged networks make the machine appear as another physical device on
  # your network.
  # config.vm.network "public_network"

  # Share an additional folder to the guest VM. The first argument is
  # the path on the host to the actual folder. The second argument is
  # the path on the guest to mount the folder. And the optional third
  # argument is a set of non-required options.
   config.vm.synced_folder "./share", "/vagrant_data"

  # Enable provisioning with a shell script. 
   config.vm.provision "shell", inline: <<-SHELL
     sudo add-apt-repository ppa:deadsnakes/ppa
     sudo apt-get update     
     sudo apt-get install golang
     sudo apt-get install python3.6
     sudo apt install python3-pip
     pip install virtualenv
     pip install requests
     pip install selenium
     pip install paramiko
     python -m pip install –upgrade pip
   SHELL
end
