# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # All Vagrant configuration is done here. The most common configuration
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "ubuntu/trusty64"

  # Fixes changes from https://github.com/mitchellh/vagrant/pull/4707
  config.ssh.insert_key = false

  # The url from where the 'config.vm.box' box will be fetched if it
  # doesn't already exist on the user's system.

  # Ubuntu 14.04 x64 VM with VirtualBox 4.3.10 Guest Additions
  # config.vm.box_url = "http://naruh.sakura.ne.jp/vagrant/ubuntu-14-04-x64-virtualbox.box"

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", 2048] # RAM allocated to each VM
  end

  config.vm.provision :shell, :path => "bootstrap.sh"

  config.vm.define :u1401 do |u1401|
    # uncomment the line below to set up the ambari dev environment
    # u1401.vm.provision :shell, :path => "dev-bootstrap.sh"
    u1401.vm.hostname = "u1401.ambari.apache.org"
    u1401.vm.network :private_network, ip: "192.168.14.101"
  end

  config.vm.define :u1402 do |u1402|
    u1402.vm.hostname = "u1402.ambari.apache.org"
    u1402.vm.network :private_network, ip: "192.168.14.102"
  end

  config.vm.define :u1403 do |u1403|
    u1403.vm.hostname = "u1403.ambari.apache.org"
    u1403.vm.network :private_network, ip: "192.168.14.103"
  end

  config.vm.define :u1404 do |u1404|
    u1404.vm.hostname = "u1404.ambari.apache.org"
    u1404.vm.network :private_network, ip: "192.168.14.104"
  end

  config.vm.define :u1405 do |u1405|
    u1405.vm.hostname = "u1405.ambari.apache.org"
    u1405.vm.network :private_network, ip: "192.168.14.105"
  end

  config.vm.define :u1406 do |u1406|
    u1406.vm.hostname = "u1406.ambari.apache.org"
    u1406.vm.network :private_network, ip: "192.168.14.106"
  end

  config.vm.define :u1407 do |u1407|
    u1407.vm.hostname = "u1407.ambari.apache.org"
    u1407.vm.network :private_network, ip: "192.168.14.107"
  end

  config.vm.define :u1408 do |u1408|
    u1408.vm.hostname = "u1408.ambari.apache.org"
    u1408.vm.network :private_network, ip: "192.168.14.108"
  end

  config.vm.define :u1409 do |u1409|
    u1409.vm.hostname = "u1409.ambari.apache.org"
    u1409.vm.network :private_network, ip: "192.168.14.109"
  end

  config.vm.define :u1410 do |u1410|
    u1410.vm.hostname = "u1410.ambari.apache.org"
    u1410.vm.network :private_network, ip: "192.168.14.110"
  end

end
