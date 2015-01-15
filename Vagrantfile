# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.define "centos01" do |centos01|
    centos01.vm.box = "chef/centos-6.5"
    centos01.vm.hostname = "centos01"
    centos01.vm.network "forwarded_port", guest: 22, host: 2222, id:'ssh', auto_correct: true
  end

  config.vm.define "centos02" do |centos02|
    centos02.vm.box = "chef/centos-6.5"
    centos02.vm.hostname = "centos02"
    centos02.vm.network "forwarded_port", guest: 22, host: 2223, id:'ssh', auto_correct: true
  end
end
