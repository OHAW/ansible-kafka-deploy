VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.ssh.insert_key = false

  end
  config.vm.define "vagrantfirst" do |vagrantfirst|
    vagrantfirst.vm.box = "ubuntu/trusty64"
    vagrantfirst.vm.network "forwarded_port", guest: 80, host: 8081
    vagrantfirst.vm.network "forwarded_port", guest: 443, host: 8443
  end
 
  config.vm.define "vagrantsecond" do |vagrantsecond|
    vagrantsecond.vm.box = "ubuntu/trusty64"
    vagrantsecond.vm.network "forwarded_port", guest: 80, host: 8082
    vagrantsecond.vm.network "forwarded_port", guest: 443, host: 8444
  end
 
  config.vm.define "vagrantthird" do |vagrantthird|
    vagrantthird.vm.box = "ubuntu/trusty64"
    vagrantthird.vm.network "forwarded_port", guest: 80, host: 8083
    vagrantthird.vm.network "forwarded_port", guest: 443, host: 8445
  end
end