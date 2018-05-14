# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|

  config.vm.box = "centos/7"
  config.vm.hostname = "scholars-backpack"
  config.vm.synced_folder ".", "/vagrant", type: "sshfs"

  config.vm.network "forwarded_port", guest: 8983, host: 5454
  config.vm.network "forwarded_port", guest: 8888, host: 5453
  config.vm.network "forwarded_port", guest: 8787, host: 5452

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = 'ansible/playbook.yml'
    ansible.inventory_path = 'ansible/inventories/development.ini'
    ansible.galaxy_role_file = 'ansible/requirements.yml'
    ansible.limit = 'all'
  end
end
