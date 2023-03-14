# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-22.04"
  config.vm.network "forwarded_port", guest: 8080, host: 8080
  config.vm.provision 'ansible', run: 'always', type: :ansible_local do |ansible|
    ansible.verbose = "v"
    ansible.galaxy_role_file = 'requirements.yml'
    ansible.playbook = 'playbook.yml'
  end
end
