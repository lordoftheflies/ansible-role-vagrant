# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'libvirt'

Vagrant.configure("2") do |config|
  ##### DEFINE VM #####
  config.vm.define "ubuntu-01" do |config|
  config.vm.hostname = "ubuntu-01"
  config.vm.box = "generic/ubuntu1804"
  config.vm.box_check_update = true
  config.vm.network "private_network", ip: "192.168.55.101"
  config.vm.provider "libvirt" do |v|
    v.memory = 1024
    end
  end
end
