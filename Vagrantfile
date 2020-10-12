
Vagrant.configure("2") do |config|

    
  config.vm.define "central" do |central|
    central.vm.box = "Gfast/Mycentral"
    config.vm.box_version = "1.0.0"
    config.vm.network :private_network, ip: "10.0.1.10"
    config.vm.network "forwarded_port", guest: 22, host: 8080    
  end
  
  config.vm.define "worker1" do |worker1|
    config.vm.box = "Gfast/Myworker"
    config.vm.box_version = "1.0.0"
    config.vm.network :private_network, ip: "10.0.1.11"
    config.vm.network "forwarded_port", guest: 22, host: 8081    
  end
  
    config.vm.box = "base"

end
