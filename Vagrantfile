Vagrant.configure("2") do |config|

    config.vm.define "agloriosS" do |master|
      master.vm.box = "generic/alpine312"
      master.vm.network "private_network", ip: "192.168.56.110"
      master.vm.hostname = "agloriosS"
      master.vm.synced_folder "./confs", "/vagrant", type:"virtualbox"
      master.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = "1"
        vb.name = "agloriosS"
      end