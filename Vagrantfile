# -*- mode: ruby -*-  
# vi: set ft=ruby :  
 
# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!  
VAGRANTFILE_API_VERSION = "2"  
 
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|  
   config.vm.define "webserver-nginx" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.205"
       app.vm.hostname = "webserver-nginx"  
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512  
           v.cpus = 1  
       end 
   end  
   config.vm.define "dbserver-mongodb" do |app|  
       app.vm.box = "debian/bullseye64"  
       app.vm.network "private_network", ip: "192.168.56.206"
       app.vm.hostname = "dbserver-mongodb"  
       app.vm.provider "virtualbox" do |v|  
           v.memory = 512  
           v.cpus = 1  
       end 
   end
end 
