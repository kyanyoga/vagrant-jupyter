# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"    
  config.vm.synced_folder "./data", "/vagrant_data"    

  # config.vm.network "private_network", ip: "192.168.50.4"
  config.vm.network "public_network", bridge: "en0: Ethernet"
    
  # configure port forwarding if private 
  # config.vm.network "forwarded_port", guest: 8888, host: 8888
  # config.vm.network "forwarded_port", guest: 4040, host: 4040

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "3072"
  end

  # config.vm.provision "shell", path: "provisioning.sh"

end
