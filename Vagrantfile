# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |global_config|

  global_config.vm.define :mac do |config|
    config.vm.box = 'jhcook/macos-sierra'

    config.vm.provider 'virtualbox' do |vb|
       # Display the VirtualBox GUI when booting the machine
       vb.gui = true

       # Customize the amount of memory on the VM:
       vb.memory = '2048'

       # Set display size
       vb.customize ['setextradata', :id, 'VBoxInternal2/EfiGopMode', '4']
    end
  end

  global_config.vm.define :win do |config|
    config.vm.box = 'peru/windows-server-2019-datacenter-x64-eval'

    config.vm.provider 'virtualbox' do |vb|
       # Display the VirtualBox GUI when booting the machine
       vb.gui = true

       # Customize the amount of memory on the VM:
       vb.memory = '2048'
    end

    config.vm.network 'public_network'
  end

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
  # config.vm.synced_folder "../data", "/vagrant_data"



  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Define a Vagrant Push strategy for pushing to Atlas. Other push strategies
  # such as FTP and Heroku are also available. See the documentation at
  # https://docs.vagrantup.com/v2/push/atlas.html for more information.
  # config.push.define "atlas" do |push|
  #   push.app = "YOUR_ATLAS_USERNAME/YOUR_APPLICATION_NAME"
  # end

  # Enable provisioning with a shell script. Additional provisioners such as
  # Puppet, Chef, Ansible, Salt, and Docker are also available. Please see the
  # documentation for more information about their specific syntax and use.

end
