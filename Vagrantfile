Vagrant.configure("2") do |config|
  # VM Database
  config.vm.define "vm-database" do |db|
    db.vm.box = "bento/ubuntu-22.04"
    db.vm.hostname = "vm-database"
    db.vm.network "private_network", ip: "192.168.56.11"
    db.vm.provider "virtualbox" do |vb|
      vb.name = "vm-database"
      vb.memory = "1024"
      vb.cpus = 1
    end
  end

  # VM Backend
  config.vm.define "vm-backend" do |backend|
    backend.vm.box = "bento/ubuntu-22.04"
    backend.vm.hostname = "vm-backend"
    backend.vm.network "private_network", ip: "192.168.56.10"
    backend.vm.provider "virtualbox" do |vb|
      vb.name = "vm-backend"
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end