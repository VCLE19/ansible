# -*- mode: ruby -*-  
# vi: set ft=ruby :  
 
# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!  
VAGRANTFILE_API_VERSION = "2"  
 
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|  
   config.vm.define "loadbalancer" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.200"  
       app.vm.hostname = "loadbalancer"  
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512  
           v.cpus = 1  
       end  
   end  
   config.vm.define "webserver-one" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.201"  
       app.vm.hostname = "webserver-one"  
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512  
           v.cpus = 1  
       end 
   end
   config.vm.define "webserver-two" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.202"
       app.vm.hostname = "webserver-two"
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512
           v.cpus = 1
       end  
   end  
   config.vm.define "dbserver" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.203"
       app.vm.hostname = "dbserver"  
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512  
           v.cpus = 1  
       end 
   end
end 