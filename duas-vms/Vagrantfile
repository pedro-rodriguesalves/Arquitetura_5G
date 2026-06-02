Vagrant.configure("2") do |config|

  config.vm.define "ran" do |ran|
    ran.vm.box = "ubuntu/jammy64"
    ran.vm.hostname = "ran"

    ran.vm.network "private_network",
      ip: "192.168.56.10"

    ran.vm.provider "virtualbox" do |vb|
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "core" do |core|
    core.vm.box = "ubuntu/jammy64"
    core.vm.hostname = "core"

    core.vm.network "private_network",
      ip: "192.168.56.11"

    core.vm.provider "virtualbox" do |vb|
      vb.memory = 4096
      vb.cpus = 2
    end
  end

end
