# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

#VAGRANT_EXPERIMENTAL="disks"
Vagrant.configure("2") do |config|
    # The most common configuration options are documented and commented below.
    # For a complete reference, please see the online documentation at
    # https://docs.vagrantup.com.
  
    # Every Vagrant development environment requires a box. You can search for
    # boxes at https://vagrantcloud.com/search.
    config.vm.box = "debian/bookworm64"
    config.vm.define "gcp" do |gcp|
        gcp.vm.network "private_network", ip: "192.168.60.10"
        #gcp.vm.network "forwarded_port", guest: 5000, host: 5000
        gcp.vm.hostname="gcp"
        gcp.vm.provision "shell",run: "always", inline: <<-SHELL                                            
            apt-get update
            apt-get install 
        SHELL
    end

end 
