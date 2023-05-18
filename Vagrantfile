# -*- mode: ruby -*-1
# vim: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/focal64"
    config.vm.provider "virtualbox" do |v|
        v.memory = 1024
        v.cpus = 1
end
    config.vm.define "nginx" do |web|
        web.vm.network "private_network", ip: "192.168.57.150"
#	web.vm.network "forwarded_port", guest: 80, host: 8080, autocorrect: true
        web.vm.hostname = "nginx"
    end
end
