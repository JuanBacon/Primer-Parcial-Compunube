Vagrant.configure("2") do |config|
  config.vm.define :servidorHaproxy do |servidorHaproxy|
  servidorHaproxy.vm.box = "bento/ubuntu-20.04"
  servidorHaproxy.vm.network :private_network, ip: "192.168.100.20"
  servidorHaproxy.vm.hostname = "servidorHaproxy"
  servidorHaproxy.vm.provision "shell", path: "scrHA.sh"
  end
  config.vm.define :servidorWeb1 do |servidorWeb1|
  servidorWeb1.vm.box = "bento/ubuntu-20.04"
  servidorWeb1.vm.network :private_network, ip: "192.168.100.30"
  servidorWeb1.vm.hostname = "servidorWeb1"
  servidorWeb1.vm.provision "shell", path: "scrWEB1.sh"
  end
  config.vm.define :servidorWeb2 do |servidorWeb2|
  servidorWeb2.vm.box = "bento/ubuntu-20.04"
  servidorWeb2.vm.network :private_network, ip: "192.168.100.40"
  servidorWeb2.vm.hostname = "servidorWeb2"
  servidorWeb2.vm.provision "shell", path: "scrWEB2.sh"
  end
  end